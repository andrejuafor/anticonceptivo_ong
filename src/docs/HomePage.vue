<template>
  <div>
    <mdb-navbar id="main-navbar" class="main-navbar2" light position="top" color="white"  scrolling :scrollingOffset="20">
      <mdb-navbar-brand to="/" waves class="font-weight-bold">
        <img class="header-logo-navbar" src="../../build/img/img-Marie/logo_page_green.png">
      </mdb-navbar-brand>
      <mdb-navbar-toggler>
        <mdb-navbar-nav center >
          <mdb-nav-item><a class="porto-button" @click="scrollMeTo('process')"><strong>Interrupción del embarazo</strong></a></mdb-nav-item> 
          <mdb-nav-item><a class="porto-button" @click="scrollMeTo('calculadora-ref')"><strong>Calcula tu tiempo de embarazo</strong></a></mdb-nav-item>
          <mdb-nav-item><a class="porto-button" @click="scrollMeTo('quest')"><strong>Preguntas frecuentas</strong></a></mdb-nav-item>
          <mdb-nav-item><a class="porto-button"><strong>Blog</strong></a></mdb-nav-item>
        </mdb-navbar-nav>
      </mdb-navbar-toggler>
    </mdb-navbar>
    <div style="margin-top: -70px;">
      <mdb-edge-header class="home-page-background">
        <div class="blue-bar">
          <div>
            <h2 class="blue-bar-title">
              Todas las mexicanas tienen el derecho al acceso a interrumpir legalmente su embarazo, dependiendo de las causales de cada estado
            </h2>
          </div>
          <div class="blue-bar-interior-wats">
            <p class="h5 contact-title">
              <!-- Contáctanos  --> &nbsp;
            </p>
              <img class="whats-icon" src="../../build/img/img-Marie/whatsappicon_blank.png">
            <p class="h5 contact-number">
              <!-- XXXXXXXXXX --> &nbsp;
            </p>
          </div>
        </div>
      </mdb-edge-header>
      <mdb-container>
        <h2 class="text-center mt-5 font-weight-bold fl-porto" ref="process">Interrupción del embarazo</h2>
        <mdb-col md="10" class="mx-auto text-center text-muted mb-5">
          <p>Antes de iniciar el proceso, considera lo siguiente</p>
        </mdb-col>
        <!-- Sección de interrupción -->
        <pm-interrupcion></pm-interrupcion>
        <h2 class="text-center mt-5 font-weight-bold">Consulta nuestra información</h2>
        <mdb-col md="10" class="mx-auto text-center text-muted mb-5">
          <p>Descarga las guías para obtener información detallada de cada paso de proceso.</p>
        </mdb-col> 
        <mdb-row>
          <a name="lancha" id="lancha" class="fadeIn"></a>
          <mdb-col md="3" class="mb-5">
            <mdb-card v-animateOnScroll="{animation: 'fadeInLeft', delay: 400}"> 
              <mdb-btn class="buttom-process" color="#FF0000" @click.native="showModal4 = true">
                <mdb-icon icon="tablets" class="fa-3x tablets-icon"/>
                <br>
                MIFE + MISO
              </mdb-btn>
            </mdb-card>
            <mdb-modal centered :show="showModal4" @close="showModal4 = false">
              <mdb-modal-header>
                <mdb-modal-title>MIFE + MISO</mdb-modal-title>
              </mdb-modal-header>
              <mdb-modal-body>
                <img style="width: 100%;" src="../../build/img/img-Marie/infografia_mife+miso_1.jpg">
              </mdb-modal-body>
              <mdb-modal-footer>
                <mdb-btn color="#FF0000" @click.native="showModal4 = false">Cerrar</mdb-btn>
              </mdb-modal-footer>
            </mdb-modal>
          </mdb-col>
          <mdb-col md="3" class="mb-5">
            <mdb-card v-animateOnScroll="{animation: 'fadeInLeft', delay: 400}"> 
              <mdb-btn class="buttom-process" color="#FF0000" @click.native="showModal = true">
                <mdb-icon icon="chevron-circle-left" class="fa-3x before-icon"/>
                <br>
                ANTES DEL PROCESO
              </mdb-btn>
            </mdb-card>
            <mdb-modal centered :show="showModal" @close="showModal = false">
              <mdb-modal-header>
                <mdb-modal-title>Antes del proceso</mdb-modal-title>
              </mdb-modal-header>
              <mdb-modal-body>
                <img style="width: 100%;" src="../../build/img/img-Marie/infografia_mife+miso_antesdelproceso.jpg">
              </mdb-modal-body>
              <mdb-modal-footer>
                <mdb-btn color="#FF0000" @click.native="showModal = false">Cerrar</mdb-btn>
              </mdb-modal-footer>
            </mdb-modal>
          </mdb-col>
          <mdb-col md="3" class="mb-5">
            <mdb-card v-animateOnScroll="{animation: 'fadeInRight', delay: 400}"> 
              <mdb-btn class="buttom-process" color="#FF0000" @click.native="showModal2 = true">
                <mdb-icon far icon="clock" class="fa-3x clock-icon"/>
                <br>
                Durante el proceso
              </mdb-btn>
            </mdb-card>
            <mdb-modal centered :show="showModal2" @close="showModal2 = false">
              <mdb-modal-header>
                <mdb-modal-title>Durante el proceso</mdb-modal-title>
              </mdb-modal-header>
              <mdb-modal-body>
                <img style="width: 100%;" src="../../build/img/img-Marie/infografia_mife+miso_proceso.jpg">
              </mdb-modal-body>
              <mdb-modal-footer>
                <mdb-btn color="#FF0000" @click.native="showModal2 = false">Cerrar</mdb-btn>
              </mdb-modal-footer>
            </mdb-modal>
          </mdb-col>
          <mdb-col md="3" class="mb-5">
            <mdb-card v-animateOnScroll="{animation: 'fadeInRight', delay: 400}"> 
              <mdb-btn class="buttom-process" color="#FF0000" @click.native="showModal3 = true">
                <mdb-icon icon="chevron-circle-right" class="fa-3x after-icon" />
                <br>
                Después del proceso
              </mdb-btn>
            </mdb-card>
            <mdb-modal centered :show="showModal3" @close="showModal3 = false">
              <mdb-modal-header>
                <mdb-modal-title>Después del proceso</mdb-modal-title>
              </mdb-modal-header>
              <mdb-modal-body>
                <img style="width: 100%;" src="../../build/img/img-Marie/infografia_mife+miso_despuesdelproceso.jpg">
              </mdb-modal-body>
              <mdb-modal-footer>
                <mdb-btn color="#FF0000" @click.native="showModal3 = false">Cerrar</mdb-btn>
              </mdb-modal-footer>
            </mdb-modal>
          </mdb-col>
        </mdb-row>
        <mdb-row>
          <h2 class="font-weight-bold fl-porto mt-5 calculadora-titulo" ref="calculadora-ref" style="width: 100%;">Calcula tu Tiempo de Embarazo</h2>
          <mdb-col md="7" class="mb-5">
            <!-- Sección Calculadora -->
            <pm-calculadora></pm-calculadora>
          </mdb-col>
          <mdb-col md="5" class="mb-5">
            <img style="width: 80%;" src="../../build/img/img-Marie/marie stopes landing-05.jpg">
          </mdb-col>
        </mdb-row>
        <h2 class="text-center mt-5 font-weight-bold fl-porto" ref="quest">Preguntas frecuentes</h2>
        <mdb-col md="8" class="mx-auto text-center mb-5" style="font-size: 15px;">
        </mdb-col>
        <mdb-accordion :panes="panes"/>
      </mdb-container>
    </div>
    <mdb-footer class="footer-section">
      <pm-footer></pm-footer>
    </mdb-footer>
  </div>
</template>

<script>
import { mdbContainer, mdbModal, mdbModalHeader, mdbModalTitle, mdbModalBody, mdbModalFooter, mdbCol, mdbRow, mdbIcon, mdbNavbarBrand, mdbNavbar, mdbNavItem, mdbNavbarNav, mdbNavbarToggler, mdbBtn, mdbEdgeHeader, mdbFooter, mdbCard, mdbCardImage, mdbCardTitle, mdbCardText, mdbCardBody, animateOnScroll, mdbAccordion} from 'mdbvue';
import PmFooter from '../components/Views/Footer.vue';
import PmInterrupcion from '../components/Views/Interrupcion.vue';
import PmCalculadora from '../components/Views/Calculadora.vue';

export default {
  name: 'HomePage',
  components: {
    PmFooter,
    PmInterrupcion,
    PmCalculadora,
    mdbContainer,
    mdbCol,
    mdbRow,
    mdbIcon,
    mdbNavbarBrand,
    mdbNavbar,
    mdbNavItem,
    mdbNavbarNav,
    mdbNavbarToggler,
    mdbBtn,
    mdbEdgeHeader,
    mdbCard,
    mdbCardImage, 
    mdbCardTitle,
    mdbCardText,
    mdbCardBody,
    mdbAccordion,
    mdbModal,
    mdbModalHeader,
    mdbModalTitle,
    mdbModalBody,
    mdbModalFooter,
    mdbFooter
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
      showModal: false,
      showModal2: false,
      showModal3: false,
      showModal4: false,
      panes: [
        {
          title: '<strong>¿Qué necesito para poder realizar mi aborto con pastillas?</strong>',
          content: 'Antes de realizarte un aborto debes tener claridad, de si efectivamente estás embarazada, la cantidad de semanas de gestación y descartar la posibilidad de un embarazo ectópico; un embarazo ectópico es aquel que se ubica fuera del útero. Este tipo de embarazo es muy poco común (no más del 1%). Se puede sospechar de un embarazo ectópico, si se observan síntomas como dolor repentino intenso y si persisten en el bajo vientre, normalmente a uno de los dos lados, sangrado vaginal, mareos o desmayos. Para corroborar con exactitud las semanas de embarazo y si el embarazo es ectópico, debes de realizarte un ultrasonido. <br><br> Si sospechas que estás embarazada y no puedes acceder al ultrasonido por razones económicas, puedes optar a realizarte un prueba de embarazo, que están a la venta en las farmacias (no importa la marca, solo hay que fijarse en la fecha de caducidad) que permiten certificar el embarazo, pero no la cantidad de semanas del mismo, o también otra opción es acudir a un laboratorio o clínica para pedir una prueba llamada Fracción Beta Gonadotrofina Coriónica Humana (Beta HCG), es importante pedirla cuantitativa para que salga la cantidad exacta de semanas de embarazo.<br> <br> FUM (Fecha de la Última Menstruación): Otra forma que es muy efectiva y sin costo, es acudir a la memoria para tener un estimado de la cantidad de semanas de gestación, es necesario calcular desde el primer día de la última menstruación o regla y ese total dividirlo por 7. No obstante, hay que tener en cuenta que este método solo le sirve a las mujeres que han tenido una menstruación regular el último año, pues puede tener un margen de error de aproximadamente dos semanas. <br><br> El procedimiento está contraindicado en el caso de que padezcas anemia severa o problemas de coagulación, como también en el hecho de haberte practicado una cesárea en los últimos 30 días; en caso de que tengas puesto un DIU (Dispositivo Intrauterino) o SIU (Sistema Intrauterino) estos deben de ser retirado antes de aplicar el método.'
        }, {
          title: '<strong>¿Qué elementos y materiales son necesarios para comenzar con la interrupción con medicamentos?<strong>',
          content: '<ul><li>Toallas sanitarias (tamaño normal) para controlar el sangrado y la salida del saco gestacional, que puede caer en la toalla, o bien, irse en los restos expulsados cada vez que vayas al baño </li><li>Analgésicos o hierbas (manzanilla, canela y orozus) para subsanar el dolor o cólicos durante el procedimiento</li><li>Dinero para movilizarse en un taxi a un centro de salud u hospital, solo en caso de emergencia (los riesgos son bajos)</li><li>Minutos en el teléfono celular para conectarse con una mujer de confianza en caso de emergencia</li></ul><br><br><strong>¿QUÉ HAY QUE TOMAR EN CUENTA ANTES DE INICIAR EL PROCEDIMIENTO?</strong><br><br><ul><li>Conocer con certeza las semanas exactas de embarazo</li><li>Lo más recomendable para saber las semanas exactas de embarazo o descartar que este sea ectópico es realizarse un ultrasonido</li><li>Padecer anemia severa, problemas de coagulación, haber vivido una cesaría durante los últimos 30 días, en todos estos casos, el aborto con medicamentos está contraindicado</li><li>Si tienes puesto un DIU (Dispositivo intrauterino), este debe ser retirado antes de iniciar el procedimiento</li><li>Estar acompañada por una mujer de confianza, que te ayude en caso de emergencia</li></ul>'
        },
        {
          title: '<strong>¿Cuáles son los tipos de procedimiento para abortar con pastillas?<strong>',
          content: '<strong>Método 1: Aborto con 12 pastillas de Misoprostol</strong><br><br>Las 12 pastillas de Misoprostol de 200mcg (microgramos), vía sublingual (debajo de la lengua) deben ser divididas en tres dosis de cuatro pastillas cada una, cada tres horas.<br>Cada dosis de cuatro pastillas juntas debe ser ingerida vía sublingual (Debajo de la lengua) pues de esta forma es absorbida más rápido y se va directamente al torrente sanguíneo.<br>Es preciso mantenerlas 30 minutos debajo de la lengua, sin tragar ni masticar durante ese periodo. <br>Los restos del medicamento se pueden escupir o tragar. Es importante insistir en que el procedimiento debe realizarse completamente, es decir, consumir las 12 pastillas de misoprostol.<br><br><strong>Método 2: Aborto con Mifepristona + Misoprostol</strong><br><br><strong>Paso 1.</strong>Tragar una tableta de 200 mg de Mifepristona con agua. Esta es dosis única. La Mifepristona bloquea e impide el acceso de la progesterona, que es la hormona que permite mantener el embarazo.<br><strong>Paso 2.</strong>Tragar 2 tabletas de Ibuprofeno de 400 mg cada una 1 hora ANTES del Misoprostol. Recuerda que la primera toma de Ibuprofeno es entre la toma de Mifepristona y Misoprostol.  El Ibuprofeno sirve para aminorar los cólicos.<br><strong>Paso 3.</strong>Colocar 4 tabletas de Misoprostol, dos entre el cachete y la encía superior izquierda, y dos entre el cachete y la encía superior derecha. Dejar pasar 30 minutos para que se absorban. Cuando pasen los 30 minutos, si aún quedan restos de las patillas, puedes pasarlos con agua. <br><strong>Paso 4.</strong>Para ayudar a disminuir las molestias, puedes continuar tomando Ibuprofeno durante 3 días más, 2 tabletas de 400 mg cada una, cada 8 horas.<br><br>'
        },
        {
          title: '<strong>¿Cuáles son los síntomas comunes asociados al consumo de las pastillas?<strong>',
          content: '<ul><li>Sangrado mayor o igual al de una menstruación, expulsión de tejidos, coágulos y saco gestacional (tejido amarillento y viscoso) (sangrado y saco gestacional)</li><li>Cólicos menstruales </li><li>Diarrea</li><li>Vómitos</li><li>Náuseas</li><li>Escalofríos (lustración “Sonrojada”)</li><li>Fiebre (Hasta 38°) durante el procedimiento</li></ul>Todos estos síntomas son considerados normales; duran entre 8 y 10 horas y pueden comenzar a presentarse hasta 72 horas después de haber colocado la primera dosis de misoprostol. Para disminuir los síntomas del cólico, el ibuprofeno es muy efectivo. Te puedes tomar dos pastillas de ibuprofeno de 400 mg, media hora antes de poner la primera dosis de misoprostol y luego ibuprofeno antes de colocar cada dosis, es decir, NO más de cinco pastillas de ibuprofeno durante todo el procedimiento. También se pueden utilizar aguas de hierbas como: manzanilla, canela y orozuz. NO se pueden tomar medicamentos que se usen normalmente para los cólicos menstruales pues reduce las contracciones en el útero y pueden contra restar el efecto del misoprostol. Tampoco se pueden utilizar: viadil y aspirina. Ni consumir alcohol o drogas durante el procedimiento.<br>También la aplicación de calor local como bolsas de agua en la panza o baños de agua caliente pueden ayudar a aminorar los síntomas del dolor. Es importante que estés hidratada con agua, te encuentres relajada y en un espacio de confianza, ya que entre menos estresada, los síntomas irán disminuyendo.'
        },
        {
          title: '<strong>¿Cuándo acudir a un centro médico u hospital?<strong>',
          content: '<ul><li><strong>Hemorragia:</strong>Se puede evidenciar cuando se llenan dos toallas sanitarias normales en una hora y en la hora siguiente dos toallas sanitarias más, acompañado de otros síntomas como, mareos, palidez extrema o desmayos.</li><li><strong>Infección:</strong>Cuando se presenta fiebre sobre los 38° luego de terminado el procedimiento (10 horas después de iniciado el sangrado), con o sin evacuación de restos con mal olor de color obscuro, que conjugan una sensación de malestar generalizado.</li><li><strong>Alergia:</strong>Cuando presentas alguna dificultad para tragar o respirar tras el consumo de misoprostol, otros síntomas de alergia, serian: hinchazón y picazón en el cuerpo. (Picazón Antihistamínico)</li></ul> El misoprostol y la mifepristona NO operan como métodos anticonceptivos, por lo tanto, después de ser usados, puedes volver a quedar embarazada. Se recomienda, por lo mismo, que si deseas evitar nuevos embarazos, uses algún método anticonceptivo de largo como el DIU, SIU o implante hormonal, además del de barrera (condón). '
        },
        {
          title: '<strong>¿Puedo abortar con misoprostol si me encuentro lactando?<strong>',
          content: ''
        },
        {
          title: '<strong>¿Se puede realizar el procedimiento más de una ocasión?<strong>',
          content: ''
        },
        {
          title: '<strong>¿Puedo beber o fumar alcohol durante el procedimiento?<strong>',
          content: 'NO, de ninguna manera puedes fumar, ingerir alcohol o alguna otra droga durante el procedimiento con Misoprostol + Mifepristona.'
        },
        {
          title: '<strong>¿En qué casos NO se puede realizar el procedimiento con Misoprostol + Mifepristona?<strong>',
          content: '<ul><li>Si tienes anemia severa</li><li>Si tienes antecedentes de alergia al misoprostol</li><li>Si tienes problemas graves de coagulación</li><li>Si tienes un dispositivo intrauterino (DIU) éste debe ser retirado antes de realizar el tratamiento</li><li>Si tienes más de 12 de gestación </li><li>Tienes un embarazo ectópico (embarazo fuera del útero)</li><li>Si sabes que NO podrás acudir a algún centro de salud en caso de emergencia</li><li>Se te practicaste una cesárea el último mes</li><li>Si estás siendo obligada a abortar</li><li>Si NO estás segura de tu decisión </li></ul>'
        }
      ]
    };
  },
  directives: {
    animateOnScroll
  },
  
  methods: {
    scrollMeTo(refName) {
      var element = this.$refs[refName];
      var top = element.offsetTop;
      window.scrollTo(0, top);
    }
  }
};

</script>

<style scoped>
h1, h2 {
  font-weight: normal;
}

.home-feature-box {
  padding: 40px 0;
}

.home-feature-box i {
  font-size: 6rem;
}

.home-feature-box span {
  display: block;
  color: black;
  font-size: 20px;
  font-weight: bold;
  padding-top: 20px;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
}

a {
  color: #42b983;
}

.home-page-background {
  width: 100%;
  height: 100%;
  background: url('../../build/img/img-Marie/fondo.jpg');
  background-size: cover;
  height: 670px; 
  position: relative;
}
.header-logo-navbar{
  max-width: 200px;
  width: 100%;
}


.whats-icon{
  margin: 0px 50px 10px;
  max-width: 60px;
}

.tablets-icon{
  margin: 10px;
}

.before-icon{
  margin: 10px;
}

.clock-icon{
  margin: 10px;
}

.after-icon{
  margin: 10px;
}

.contact-title{
  color: white; 
  text-align:center; 
  padding:3px 3px;
}

.contact-number{
  color: white; 
  text-align:center; 
  padding:3px 3px;
}

.phone-number{
  color: white;
  font-weight: bold;
  font-size: 18px;
  margin-left: -22px;
}

.input-secction{
    display: block;
    top: 555px;
    width: 10%;
    height: 20%;
    background-color: rgba(0,0,0,.5);;
    padding: 30px;
    margin-right: 100px;
}

.buttom-process{
  background: #019934;
  border: 0px;
  height: 100px;
  border-radius: 6px 6px 6px 6px;
  -moz-border-radius: 6px 6px 6px 6px;
  -webkit-border-radius: 6px 6px 6px 6px;
  color: white;
  font-weight: bold;
}

.form-section{
  border: #000000;
}


.form-extra{
  padding: 0% 0% 20% 1%;;
}

.blue-bar {
  position: absolute; 
  bottom: 0; 
  display:flex; 
  justify-content: space-between;
  background-color: rgba(0, 43, 83, 0.9);
}

.blue-bar-interior-wats{
  padding: 5px 20px;
}

.blue-bar-title{
  color: white; 
  padding: 45px 5px 0px 30px;
  font-weight: normal;
  font-size: 25px;
}

.porto-button{
  color: #019934 !important;
  margin-right: 10px;
}

.footer-section{
  background: #1f1e1e;
  color: white;
}

.more-infro-buttom{ 
  font-size: 15px;
}

@media (max-width: 766px) {
  .home-page-background {
    width: 100%;
    height: 100%;
    background: url(/static/img/fondo.676f4bb.jpg);
    background-size: contain;
    background-repeat: no-repeat;
    height: 487px;
    position: relative;
    background-attachment: inherit;
    margin-top: 94px;
    background-position: 0 67px;
  }
  .input-secction{
    width: 100%;
    top: 80px;
    padding: 50px;
  }
  .phone-number{
    color:white;
    font-weight: bold;
    font-size: 20px;
    margin-left: 50px;
  }
  
  .blue-bar{
    text-align: center;
  }
  .blue-bar-title{
    padding: 10px 0px 0px 0px;
    font-size: 25px;
    display: flex;
    flex-wrap: wrap;
    text-align: center;
  }
  .blue-bar-interior-wats{
    padding: 5px 20px;
  }
  .blue-bar-subtitle{
    padding: 5px 0px 0px 0px;
    font-size: 10px;
  }
  .footer-section{
    background: #1f1e1e;
    color: white;
  }
}

@media (max-width: 1024px) {
  .input-secction{
    width: 100%;
    height: 10%;
    top: 500px;
    padding-top: 50px; 
    margin-right: 30px;
  }
  .contact-title{
    color: white; 
    text-align: left; 
    padding:3px 3px;
  }
  .contact-title{
    color: white; 
    text-align: left; 
    padding:0px 3px;
  }
  .contact-number{
    margin-top: -30px;
    margin-left: 70px;
    font-size:40px;
  }
  .whats-icon{
    margin: 0px -100px -25px -350px;
    max-width: 60px;
  }
  .blue-bar{
    text-align: center;
    display: inline-block;
  }
  .blue-bar-title{
    padding: 14px 20px 0px 20px;
    font-size: 18px;
    text-align: justify;
  }
  .blue-bar-subtitle{
    padding: 0px;
  }
  .footer-section{
    background: #1f1e1e;
    color: white;
  }
  .phone-number{
    font-size: 40px;
    margin: -63px 0px 0px 45px;
  }
}

</style>
