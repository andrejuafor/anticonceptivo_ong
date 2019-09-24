<template>
    <div>
        <h3>Esta calculadora es para saber cuántas semanas de embarazo tienes aproximadamente. En las casillas coloca la fecha de inicio de tu último periodo menstrual.</h3>
        <br />
        <select class="calculator" v-model="selectedDay">
            <option value="">Día</option>
            <option v-for="option in optionsDays" v-bind:key="option.value">{{option.text}}</option>
        </select>
        <select class="calculator" v-model="selectedMonth">
            <option value="">Mes</option>
            <option v-for="option in optionsMonth" v-bind:key="option.valor" :value="option.valor">{{option.text}}</option>
        </select>
        <select class="calculator" v-model="selectedYear">
            <option value="">Año</option>
            <option v-for="option in optionsYear" v-bind:key="option.value">{{option.text}}</option>
        </select>
        <button class="calculato-buttom" @click="calculator()">Calcular</button>
        <br>
        <br>
        <mdb-card-text>
            <strong style="font-size: 20px; font-weight: bold;">Semanas de embarazo:</strong>
            <strong style="color: #019934; font-size: 30px; font-weight: bold;">{{Results}}</strong><br>
        </mdb-card-text>
    </div>
</template>
<script>
import {mdbCardText} from 'mdbvue';
import moment from 'moment';
export default {
  name: "Calculadora",
  components:{
    mdbCardText
  },
  data() {
    return {
      optionsDays:[],
      optionsMonth:[],
      optionsYear:[],
      selectedDay: '',
      selectedMonth: '',
      selectedYear: '',
      diasMes: 31,
      Results: '',
    };
  },
  created(){
    for (let i=1; i<=31; i++) {
      this.optionsDays.push({ text:i, value:i});
    }
    this.optionsMonth = [
      {text:'Enero', valor: '01'},
      {text:'Febrero', valor: '02'},
      {text:'Marzo', valor: '03'},
      {text:'Abril', valor: '04'},
      {text:'Mayo', valor: '05'},
      {text:'Junio', valor: '06'},
      {text:'Julio', valor: '07'},
      {text:'Agosto', valor: '08'},
      {text:'Septiembre', valor: '09'},
      {text:'Octubre', valor: '10'},
      {text:'Noviembre', valor: '11'},
      {text:'Diciembre', valor: '12'}
    ];
    // let ahora = moment().format('YYYY-MM-DD');
    let diferenciaMeses = moment().subtract(9, 'months')
      .format('YYYY');
    let anioActual = moment().format('YYYY');
    if (diferenciaMeses < anioActual){
      this.optionsYear.push({text:diferenciaMeses, value:diferenciaMeses});
    }
    this.optionsYear.push({text:anioActual, value:anioActual});
  },
  methods: {
    calculator(){
      if (this.selectedDay !== '' && this.selectedMonth !== '' && this.selectedYear !== ''){
        let fechaSel = moment(`${this.selectedYear}-${this.selectedMonth}-${this.selectedDay}`, 'YYYY-MM-DD');
        let fechaValida = fechaSel.isValid();
        if (fechaValida === false){
          this.Results = 'Debes seleccionar una fecha válida.';  
        } else {
          let ahora = moment();
          let diferencia = ahora.diff(fechaSel, 'weeks');
          this.Results = `${diferencia}`;
        }
      } else {
        this.Results = 'Debes seleccionar una fecha válida.';
      }
    }
  }
};
</script>

<style scoped>
h3{
  margin-top: 15px;
  font-weight: bolder;
}
.calculator {
  background: white;
  padding: 10px 30px 10px 10px;
  border-radius: 6px 6px 6px 6px;
  -moz-border-radius: 6px 6px 6px 6px;
  -webkit-border-radius: 6px 6px 6px 6px;
}

.calculato-buttom{
  width: 15%; 
  background: #019934; 
  border-radius: 6px 6px 6px 6px;
  -moz-border-radius: 6px 6px 6px 6px;
  -webkit-border-radius: 6px 6px 6px 6px;
  border: 0px solid #000000;
  font-size: 15px;
  color: white;
  font-weight: bold;
  padding: 10px;
}
@media (max-width: 766px) {
  .calculato-buttom{
    width: 100%;
    margin-top: 10px;
  }
}
@media (max-width: 1024px) {
  .calculato-buttom{
    width: 100%;
    margin-top: 10px;
  }
  .calculadora-titulo{
    padding-left: 15px;
  }
}
</style>