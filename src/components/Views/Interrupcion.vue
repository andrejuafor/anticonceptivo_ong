<template>
    <div>
        <mdb-row>
            <mdb-col md="6" class="mb-5">
                <mdb-card class="animated fadeInLeft card-text-content">
                    <mdb-card-body style="height: 220px;" >
                    <mdb-card-title><img style="width: 8%; padding-right: 5px;" src="../../../build/img/img-Marie/marie stopes landing-06.jpg"><strong style="font-size: 18px;">Antes de iniciar con el proceso. considera lo siguiente:</strong></mdb-card-title>
                    <mdb-card-text>
                        <strong>1.Confirma que estás embarazada</strong>
                        <br>
                        ¿Cómo saber si estás embarazada?
                        <br>
                        <strong>Síntomas:</strong>
                        <br>
                        <mdb-icon icon="caret-right" /> Retraso del periodo menstrual <br>
                        <mdb-icon icon="caret-right" /> Mayor sensibilidad en los senos <br>
                        <a class="more-infro-buttom" style="color: green; " @click="showMoreInfo = true">Leer mas...</a>
                    </mdb-card-text>
                    </mdb-card-body>
                </mdb-card>
                <mdb-modal centered :show="showMoreInfo" @close="showMoreInfo = false">
                    <mdb-modal-header>
                    <mdb-modal-title><strong>Antes de iniciar con el proceso. considera lo siguiente</strong></mdb-modal-title>
                    </mdb-modal-header>
                    <mdb-modal-body> 
                        <strong>1.Confirma que estás embarazada</strong>
                        <br>
                        ¿Cómo saber si estás embarazada?
                        <br>
                        <strong>Síntomas:</strong>
                        <br><br>
                        <li>
                        <ul><mdb-icon icon="caret-right" /> Retraso del periodo menstrual</ul>
                        <ul><mdb-icon icon="caret-right" /> Mayor sensibilidad en los senos</ul>
                        <ul><mdb-icon icon="caret-right" /> Náuseas y/o vómito, especialmente al despertar </ul>
                        <ul><mdb-icon icon="caret-right" /> Dolor de cabeza</ul>
                        <ul><mdb-icon icon="caret-right" /> Cansancio</ul>
                        <ul><mdb-icon icon="caret-right" /> Orinar con mucha frecuencia</ul>
                        </li>
                        <br>
                        Poniendo atención a estos síntomas, puedes hacer una comparación después de haber usado las pastillas.
                        <br>
                        Puedes confirmar con una prueba de orina de farmacia. Para mayor certeza y para conocer la edad gestacional, puedes realizar un ultrasonido.
                        <br>
                        <br>
                        <mdb-icon icon="check" class="fa-sm"/> Pensar en los síntomas que tienes antes de iniciar el proceso ayudará a confirmar que todo salió bien después de las pastillas.
                        <br>
                        <br>
                        <strong>2. Asegúrate de que el embarazo está dentro del útero</strong>
                        <br>
                        <br>
                        Si además sientes dolor intenso que se concentra en un lado (bajo vientre derecho o bajo vientre izquierdo), que se presenta de repente, con palpitaciones y debilidad ¡requieres atención médica urgente y no puedes iniciar el proceso!
                        <br>
                        <br>
                        <mdb-icon icon="check" class="fa-sm"/> Confirma que NO se trate de un embarazo ectópico con un ultrasonido 
                        <br><br>
                        <strong>3. La edad gestacional </strong>
                        <br> 
                        ¿Cuántas semanas de embarazo tienes?
                        <br><br>
                        Puedes calcularlo de la siguiente forma: contar los días desde el primer día de la fecha de la última menstruación, el resultado en días divídelo entre siete para conocer las semanas. Si es posible, confirma con ultrasonido.
                        <br><br>
                        <mdb-icon icon="check" class="fa-sm"/> El uso del tratamiento se recomienda hasta la semana 9 de gestación.
                        <br><br>
                        <strong>4. Importante…</strong>
                        <br><br>
                        <strong>¿Tienes colocado algún dispositivo intrauterino (DIU o SIU)?</strong>
                        <br>
                        En caso de tener alguno, debes retirarlo antes de tomar las pastillas.
                        <strong>¿Eres alérgica a la mifepristona o al misoprostol?</strong>
                        <br>
                        Si eres alérgica a las pastillas, no las tomes y considera otra opción para tu interrupción 
                        <br>
                        <strong>¿Tienes problemas de coagulación, padeces anemia severa, asma no controlada o usas corticoides?</strong>
                        <br>
                        Para iniciar el proceso con las pastillas requieres vigilancia médica 
                        <br><br>
                        <strong>Recomendación:</strong>
                        <br>
                        Tener un espacio seguro y cómodo para llevar a cabo tu interrupción es importante para que te sientas tranquila, procura tener un baño cerca y suficientes toallas regulares (no nocturnas) para monitorear el sangrado. Estar acompañada de alguien en quien confías y que pueda apoyarte, facilitará el proceso. 
                        <br><br>
                        <mdb-icon icon="check" class="fa-sm"/> Identifica algún centro de salud cercano para acudir en caso de emergencia.
                    <!-- <img style="width: 100%;" src="../../build/img/img-Marie/marie stopes landing-03.jpg"> -->
                    </mdb-modal-body>
                    <mdb-modal-footer>
                    <mdb-btn color="#FF0000" @click.native="showMoreInfo = false">Cerrar</mdb-btn>
                    </mdb-modal-footer>
                </mdb-modal>
            </mdb-col>
            <mdb-col md="6" class="mb-5">
                <mdb-card class="animated fadeInRight card-text-content">
                    <mdb-card-body>
                    <mdb-card-title><img style="width: 8%; padding-right: 8px;" src="../../../build/img/img-Marie/marie stopes landing-09.jpg"><strong style="font-size: 18px;">Aborto con Mifepristona + Misoprostol</strong></mdb-card-title>
                    <mdb-card-text>
                        <strong> Paso 1.</strong>Tragar una tableta de 200 mg de Mifepristona con agua. Esta es dosis única. La Mifepristona bloquea e impide el acceso de la progesterona, que es la hormona que permite mantener el embarazo.
                        <br>
                        <strong>Paso 2.</strong>Tragar 2 tabletas de Ibuprofeno de 400 mg cada una 1 hora ANTES del Misoprostol. Recuerda que la primera toma de Ibuprofeno es entre la toma de Mifepristona y Misoprostol.
                        <a class="more-infro-buttom" style="color: green;" @click="showMoreInfo2 = true">Leer mas...</a>
                    </mdb-card-text>
                    </mdb-card-body>
                </mdb-card>
                <mdb-modal centered :show="showMoreInfo2" @close="showMoreInfo2 = false">
                    <mdb-modal-header>
                    <mdb-modal-title>Aborto con Mifepristona + Misoprosto</mdb-modal-title>
                    </mdb-modal-header>
                    <mdb-modal-body>
                    <mdb-card-text>
                        <strong> Paso 1.</strong>Tragar una tableta de 200 mg de Mifepristona con agua. Esta es dosis única. La Mifepristona bloquea e impide el acceso de la progesterona, que es la hormona que permite mantener el embarazo.
                        <br><br>
                        <strong>Paso 2.</strong>Tragar 2 tabletas de Ibuprofeno de 400 mg cada una 1 hora ANTES del Misoprostol. Recuerda que la primera toma de Ibuprofeno es entre la toma de Mifepristona y Misoprostol. El Ibuprofeno sirve para aminorar los cólicos.
                        <br><br>
                        <strong>Paso 3.</strong>Colocar 4 tabletas de Misoprostol, dos entre el cachete y la encía superior izquierda, y dos entre el cachete y la encía superior derecha. Dejar pasar 30 minutos para que se absorban. Cuando pasen los 30 minutos, si aún quedan restos de las patillas, puedes pasarlos con agua.
                        <br><br>
                        <strong>Paso 4.</strong>Para ayudar a disminuir las molestias, puedes continuar tomando Ibuprofeno durante 3 días más, 2 tabletas de 400 mg cada una, cada 8 horas.
                    </mdb-card-text>
                    </mdb-modal-body>
                    <mdb-modal-footer>
                    <mdb-btn color="#FF0000" @click.native="showMoreInfo2 = false">Cerrar</mdb-btn>
                    </mdb-modal-footer>
                </mdb-modal>
            </mdb-col>
        </mdb-row>
        <mdb-row>
            <mdb-col md="6" class="mb-5">
            <mdb-card class="animated fadeInLeft card-text-content">
                <mdb-card-body>
                <mdb-card-title><img style="width: 8%; padding-right: 8px;" src="../../../build/img/img-Marie/marie stopes landing-07.jpg"><strong style="font-size: 18px;">Lo más frecuente…</strong></mdb-card-title>
                <mdb-card-text>Es que la expulsión ocurra en las primeras 4 horas, sin embargo se trata de un proceso en el que el útero se irá limpiando con el paso de los días , es por esta razón que el sangrado puede extenderse de 14 hasta 30 días, aproximadamente. También es importante que recuerdes cómo te sentías antes de tomar las pastillas, piensa en los síntomas que se han ido días después de usarlas.
                <a class="more-infro-buttom" style="color: green;" @click="showMoreInfo3 = true">Leer mas...</a>
                </mdb-card-text>
                </mdb-card-body>
            </mdb-card>
            <mdb-modal centered :show="showMoreInfo3" @close="showMoreInfo3 = false">
                <mdb-modal-header>
                <mdb-modal-title>Lo más frecuente…</mdb-modal-title>
                </mdb-modal-header>
                <mdb-modal-body>
                <mdb-card-text>
                    <strong>Lo más frecuente…</strong>
                    <br>
                    es que la expulsión ocurra en las primeras 4 horas, sin embargo se trata de un proceso en el que el útero se irá limpiando con el paso de los días , es por esta razón que el sangrado puede extenderse de 14 hasta 30 días, aproximadamente. También es importante que recuerdes cómo te sentías antes de tomar las pastillas, piensa en los síntomas que se han ido días después de usarlas.
                    <br><br>
                    Por ejemplo: <br>
                    <mdb-icon icon="caret-right" /> Ausencia de sangrado (esto es lo primero que notarás diferente). <br>
                    <mdb-icon icon="caret-right" /> EL DÍA QUE COLOQUES EL MISOPROSTOL, EL SANGRADO VOLVERÁ<br>
                    <mdb-icon icon="caret-right" /> Dolor de senos<br>
                    <mdb-icon icon="caret-right" /> Náuseas y/o vómito<br> 
                    <mdb-icon icon="caret-right" /> Dolor de Cabeza<br>
                    <mdb-icon icon="caret-right" /> Cansancio y/o sueño<br> 
                    <br>
                    A los 5 días de haber usado las pastillas, notarás que estos síntomas van desapareciendo.
                    <br><br>
                    <strong>Después de 14 días…</strong><br>
                    Con ayuda de la prueba de embarazo, podrás confirmar la interrupción, pero si te sientes más tranquila, puedes corroborar con ultrasonido.
                    <br><br>
                    <strong>¿Cómo usar prueba de orina?</strong><br> 
                    1. Coloca un poco de orina en un recipiente desechable <br>
                    2. Una vez abierta tu prueba, sujeta con tus dedos el extremo  de color y no toques el extremo blanco.<br>
                    3. Sumerge en la orina el extremo blanco hasta la línea de color durante un minuto<br>
                    4. Retira la prueba de la orina y espera un minuto mientras arroja el resultado <br>
                    <br><br>
                    <strong>Resultado</strong> <br>
                    Si solo aparece una línea, tu prueba es <strong>negativa</strong><br>
                    Si observas <strong>dos líneas</strong>, el resultado es <strong>positivo</strong>. En caso de que sea positivo, comprueba con un ultrasonido. Si el resultado definitivo es positivo, es necesario evaluar una segunda dosis de medicamento o hacer un procedimiento de aspiración.
                </mdb-card-text>
                </mdb-modal-body>
                <mdb-modal-footer>
                <mdb-btn color="#FF0000" @click.native="showMoreInfo3 = false">Cerrar</mdb-btn>
                </mdb-modal-footer>
            </mdb-modal>
            </mdb-col>
            <mdb-col md="6" class="mb-5">
            <mdb-card class="animated fadeInRight card-text-content-extra card-text-content">
                <mdb-card-body>
                <mdb-card-title><img style="width: 8%; padding-right: 8px;" src="../../../build/img/img-Marie/marie stopes landing-08.jpg"><strong style="font-size: 18px;">¡Datos de alarma!</strong></mdb-card-title>
                <mdb-card-text ><br>
                    <mdb-icon icon="caret-right" /> Continuación del embarazo. <br>
                    <mdb-icon icon="caret-right" /> Presencia de alguna infección <br>
                    <mdb-icon icon="caret-right" /> Sangrado mayor al esperad <br>
                </mdb-card-text>
                </mdb-card-body>
            </mdb-card>
            </mdb-col>
        </mdb-row>
    </div>
</template>

<script>
import { 
  mdbContainer, 
  mdbModal, 
  mdbModalHeader, 
  mdbModalTitle,
  mdbModalBody, 
  mdbCol,
  mdbRow,
  mdbModalFooter,
  mdbIcon, mdbBtn, mdbCard, mdbCardTitle, mdbCardText, mdbCardBody } from 'mdbvue';
export default {
  name: 'Interrupicion',
  components: {
    mdbModalFooter,
    mdbContainer,
    mdbCol,
    mdbRow,
    mdbIcon,
    mdbBtn,
    mdbCard,
    mdbCardTitle,
    mdbCardText,
    mdbCardBody,
    mdbModal,
    mdbModalHeader,
    mdbModalTitle,
    mdbModalBody
  },
  data() {
    return {
      showMoreInfo: false,
      showMoreInfo2: false,
      showMoreInfo3: false,
    };
  }
};
</script>

<style scoped>
.card-text-content{
  height: 210px;
}
ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
}
@media (max-width: 766px) {
  .card-text-content{
    height: 300px;
  }
  .card-text-content-extra{
    height: 350px;
  }
  .calculadora-titulo{
    padding-left: 15px;
  }
}

@media (max-width: 1024px) {
  .card-text-content{
    height: 300px;
  }
  .card-text-content-extra{
    height: 350px;
  }
}
</style>

