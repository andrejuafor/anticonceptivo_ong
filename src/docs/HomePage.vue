<template>
  <div>
    <mdb-navbar id="main-navbar" class="main-navbar2" dark position="top" color="black"  scrolling :scrollingOffset="20">
      <mdb-navbar-brand to="/" waves class="font-weight-bold">
        <img class="header-logo-navbar" src="../../build/img/img-Marie/logo_page.png">
      </mdb-navbar-brand>
      <mdb-navbar-toggler>
        <mdb-navbar-nav center >
          <mdb-nav-item><a class="porto-button" @click="scrollMeTo('process')"><strong>Interrupcion Del Embarazo</strong></a></mdb-nav-item> 
          <mdb-nav-item><a class="porto-button" @click="scrollMeTo('calculadora-ref')"><strong>Calcula tu Tiempo de Embarazo</strong></a></mdb-nav-item>
          <mdb-nav-item><a class="porto-button" @click="scrollMeTo('quest')"><strong>Preguntas frecuentas</strong></a></mdb-nav-item>
        </mdb-navbar-nav>
      </mdb-navbar-toggler>
    </mdb-navbar>
    <!-- :style="{marginTop: '60px'}" -->
    <div style="margin-top: -60px;">
      <mdb-edge-header style="height: 670px;">
        <div align="right" class="home-page-background">
          <mdb-col align="left" class="input-secction" sm="6">
            <p class="h4" style="color: white;">Contáctanos</p>
            <img class="whats-icon" src="../../build/img/img-Marie/whatsappicon.png">
            <p class="phone-number">5614737334</p>
          </mdb-col>
        </div>
        <div class="blue-bar">
          <section style="background: #002B53; height: 19%; margin-top: -110px;">
            <h2 class="blue-bar-title">Di sí al amor, pero con anticonceptivo dual</h2>
            <p class="blue-bar-subtitle">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.</p>
          </section>
        </div>
      </mdb-edge-header>
      <mdb-container>
        <h2 class="text-center mt-5 font-weight-bold fl-porto" ref="process">Interrupcion Del Embarazo</h2>
        <mdb-col md="10" class="mx-auto text-center text-muted mb-5">
          <p>Antes de iniciar el proceso, considera lo siguiente</p>
        </mdb-col>

        <mdb-row>
          <mdb-col md="6" class="mb-5">
            <mdb-card class="animated fadeInLeft card-text-content">
              <mdb-card-body style="height: 220px;" >
                <mdb-card-title><img style="width: 8%; padding-right: 5px;" src="../../build/img/img-Marie/marie stopes landing-06.jpg"><strong style="font-size: 20px;">CONFIRMA QUE ESTAS EMBARAZADA</strong></mdb-card-title>
                <mdb-card-text>Poniendo atención a los síntomas puedes hacer una comparación después de haber usado las pastillas. <br/><br/> Puedes confirmar con una prueba de orina de farmacia. 
                Para mayor certeza y oara conocer la edad gestional. puedes realizar un ultrasonido.</mdb-card-text>
              </mdb-card-body>
            </mdb-card>
          </mdb-col>
          <mdb-col md="6" class="mb-5">
            <mdb-card class="animated fadeInRight card-text-content">
              <mdb-card-body>
                <mdb-card-title><img style="width: 8%; padding-right: 8px;" src="../../build/img/img-Marie/marie stopes landing-09.jpg"><strong style="font-size: 20px;">ASEGÚRATE DE QUE EL EMBARAZO ESTÁ DENTRO DEL ÚTERO</strong></mdb-card-title>
                <mdb-card-text>Si además sientes dolor intenso que se concentra en un lado (bajo vientre derecho o izquierdo), 
                  que se presenta de repente, con palpitaciones y debilidad <strong style="color: #00B3E8">¡requieres atención médica urgente y no puedes iniciar el proceso!</strong></mdb-card-text>
              </mdb-card-body>
            </mdb-card>
          </mdb-col>
        </mdb-row>
        <mdb-row>
          <mdb-col md="6" class="mb-5">
            <mdb-card class="animated fadeInLeft card-text-content">
              <mdb-card-body>
                <mdb-card-title><img style="width: 8%; padding-right: 8px;" src="../../build/img/img-Marie/marie stopes landing-07.jpg"><strong style="font-size: 20px;">LA EDAD GESTIONAL</strong></mdb-card-title>
                <mdb-card-text>¿Cuantas semanas de embarazo tienes?<br><br>Puedes calcularlo de la siguiente forma: contar los dias desde el primer día de la decha de la última menstrución,
                el resultado en días divídelo entre 7 para conocer las semanas. Si es posible, confima con ulrasonido</mdb-card-text>
              </mdb-card-body>
            </mdb-card>
          </mdb-col>
          <mdb-col md="6" class="mb-5">
            <mdb-card class="animated fadeInRight card-text-content-extra">
              <mdb-card-body>
                <mdb-card-title><img style="width: 8%; padding-right: 8px;" src="../../build/img/img-Marie/marie stopes landing-08.jpg"><strong style="font-size: 20px;">IMPORTANTE</strong></mdb-card-title>
                <mdb-card-text><strong style="color: #00B3E8">¿Tienes colocado algún dispositivo intrauterino (DIU o SIU)?</strong><br>
                En caso de tener alguno, debes retirarlo antes de tomar las pastillas. <br>
                <strong style="color: #00B3E8">¿Eres alérgica a la mifepristona o al misoprostol?</strong><br>
                Si eres alérgica, no las tomes y considera otra opcion para tu interrupcion. <br>
                <strong style="color: #00B3E8">¿Tienes problemas de coagulación, padeces anemia severa, asma no controlada o usas corticoides?</strong><br>
                Para iniciar el proceso con las pastillas rquieres vigilancia médica.<br>
                </mdb-card-text>
              </mdb-card-body>
            </mdb-card>
          </mdb-col>
        </mdb-row>
        <h2 class="text-center mt-5 font-weight-bold">CONSULTA NUESTRA INFORMACIÓN</h2>
        <mdb-col md="10" class="mx-auto text-center text-muted mb-5">
          <p>Descarga nuestras guías para obtener información util de cada estatus del proceso</p>
        </mdb-col> 
        <mdb-row>
          <a name="lancha" id="lancha" class="fadeIn"></a>
          <mdb-col md="4" class="mb-5">
            <mdb-card v-animateOnScroll="{animation: 'fadeInLeft', delay: 400}"> 
              <mdb-btn class="buttom-process" color="#FF0000" @click.native="showModal = true">
                <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="50" height="50" viewBox="0 0 172 172" style=" fill:#000000; padding-bottom: 5px;">
                  <g fill="none" fill-rule="nonzero" stroke="none" stroke-width="1" stroke-linecap="butt" stroke-linejoin="miter" stroke-miterlimit="10" stroke-dasharray="" stroke-dashoffset="0" font-family="none" font-weight="none" font-size="none" text-anchor="none" style="mix-blend-mode: normal">
                    <path d="M0,172v-172h172v172z" fill="none">
                    </path>
                    <g fill="#ffffff">
                      <g id="surface1">
                        <path d="M86,6.88c-43.65844,0 -79.12,35.46156 -79.12,79.12c0,43.65844 35.46156,79.12 79.12,79.12c43.65844,0 79.12,-35.46156 79.12,-79.12c0,-43.65844 -35.46156,-79.12 -79.12,-79.12zM86,13.76c39.93625,0 72.24,32.30375 72.24,72.24c0,39.93625 -32.30375,72.24 -72.24,72.24c-39.93625,0 -72.24,-32.30375 -72.24,-72.24c0,-39.93625 32.30375,-72.24 72.24,-72.24zM95.89,48.16c-0.76594,0.08063 -1.49156,0.43 -2.0425,0.9675l-34.4,34.4c-0.67187,0.645 -1.04812,1.54531 -1.04812,2.4725c0,0.92719 0.37625,1.8275 1.04812,2.4725l34.4,34.4c1.37063,1.37063 3.57438,1.37063 4.945,0c1.37063,-1.37062 1.37063,-3.57437 0,-4.945l-31.9275,-31.9275l31.9275,-31.9275c1.11531,-1.03469 1.41094,-2.67406 0.73906,-4.03125c-0.65844,-1.37062 -2.15,-2.12312 -3.64156,-1.88125z">
                        </path>
                      </g>
                    </g>
                  </g>
                </svg>
                <br>
                Antes del proceso
              </mdb-btn>
            </mdb-card>
            <mdb-modal centered :show="showModal" @close="showModal = false">
              <mdb-modal-header>
                <mdb-modal-title>Antes del proceso</mdb-modal-title>
              </mdb-modal-header>
              <mdb-modal-body>
                <p>
                  <strong>ANTES DE INICIAR CON EL PROCESO, CONSIDERA LO SIGUENTE:</strong> 
                  <br><br>
                  <strong>1.Confirma que estás embarazada</strong>
                  <br>
                  ¿Cómo saber si estás embarazada?
                  <br>
                  <strong>Síntomas:</strong>
                  <br><br>
                  <li>
                    <ul>- Retraso del periodo menstrual</ul>
                    <ul>- Mayor sensibilidad en los senos</ul>
                    <ul>- Náuseas y/o vómito, especialmente al despertar </ul>
                    <ul>- Dolor de cabeza</ul>
                    <ul>- Cansancio</ul>
                    <ul>- Orinar con mucha frecuencia</ul>
                  </li>
                  <br>
                  Poniendo atención a estos síntomas, puedes hacer una comparación después de haber usado las pastillas.
                  <br>
                  Puedes confirmar con una prueba de orina de farmacia. Para mayor certeza y para conocer la edad gestacional, puedes realizar un ultrasonido.
                  <br>
                  <br>
                  <img src="https://img.icons8.com/metro/26/000000/checkmark.png"> Pensar en los síntomas que tienes antes de iniciar el proceso ayudará a confirmar que todo salió bien después de las pastillas.
                  <br>
                  <br>
                  <strong>2. Asegúrate de que el embarazo está dentro del útero</strong>
                  <br>
                  <br>
                  Si además sientes dolor intenso que se concentra en un lado (bajo vientre derecho o bajo vientre izquierdo), que se presenta de repente, con palpitaciones y debilidad ¡requieres atención médica urgente y no puedes iniciar el proceso!
                  <br>
                  <br>
                  <img src="https://img.icons8.com/metro/26/000000/checkmark.png"> Confirma que NO se trate de un embarazo ectópico con un ultrasonido 
                  <br><br>
                  <strong>3. La edad gestacional </strong>
                  <br> 
                  ¿Cuántas semanas de embarazo tienes?
                  <br><br>
                  Puedes calcularlo de la siguiente forma: contar los días desde el primer día de la fecha de la última menstruación, el resultado en días divídelo entre siete para conocer las semanas. Si es posible, confirma con ultrasonido.
                  <br><br>
                  <img src="https://img.icons8.com/metro/26/000000/checkmark.png"> El uso del tratamiento se recomienda hasta la semana 9 de gestación.
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
                  <img src="https://img.icons8.com/metro/26/000000/checkmark.png">Identifica algún centro de salud cercano para acudir en caso de emergencia.
                </p>
                <!-- <img style="width: 100%;" src="../../build/img/img-Marie/marie stopes landing-03.jpg"> -->
              </mdb-modal-body>
              <mdb-modal-footer>
                <mdb-btn color="green">Descargar</mdb-btn>
                <mdb-btn color="#FF0000" @click.native="showModal = false">Cerrar</mdb-btn>
              </mdb-modal-footer>
            </mdb-modal>
          </mdb-col>
          <mdb-col md="4" class="mb-5">
            <mdb-card v-animateOnScroll="{animation: 'fadeIn', delay: 400}"> 
              <mdb-btn class="buttom-process" color="#FF0000" @click.native="showModal2 = true">
                <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="50" height="50" viewBox="0 0 172 172" style=" fill:#000000;">
                  <g fill="none" fill-rule="nonzero" stroke="none" stroke-width="1" stroke-linecap="butt" stroke-linejoin="miter" stroke-miterlimit="10" stroke-dasharray="" stroke-dashoffset="0" font-family="none" font-weight="none" font-size="none" text-anchor="none" style="mix-blend-mode: normal">
                    <path d="M0,172v-172h172v172z" fill="none"></path>
                    <g fill="#ffffff">
                      <path d="M86,18.14063c-37.35625,0 -67.85937,30.50313 -67.85937,67.85938c0,37.35625 30.50313,67.85938 67.85938,67.85938c37.35625,0 67.85938,-30.50312 67.85938,-67.85937c0,-37.35625 -30.50312,-67.85937 -67.85937,-67.85937zM86,26.20313c32.92188,0 59.79688,26.875 59.79688,59.79688c0,32.92188 -26.875,59.79688 -59.79687,59.79688c-32.92187,0 -59.79687,-26.875 -59.79687,-59.79687c0,-32.92187 26.875,-59.79687 59.79688,-59.79687zM86,41.65625c-2.28437,0 -4.03125,1.74687 -4.03125,4.03125v33.32605c-2.41875,1.34375 -4.03125,4.0302 -4.03125,6.98645c0,4.43438 3.62812,8.0625 8.0625,8.0625c2.95625,0 5.6427,-1.6125 6.98645,-4.03125h19.88855c2.28437,0 4.03125,-1.74688 4.03125,-4.03125c0,-2.28437 -1.74688,-4.03125 -4.03125,-4.03125h-19.88855c-0.67187,-1.20937 -1.74583,-2.28333 -2.9552,-2.9552v-33.32605c0,-2.28438 -1.74688,-4.03125 -4.03125,-4.03125z">
                      </path>
                    </g>
                  </g>
                </svg>
                <br>
                Durante el proceso
              </mdb-btn>
            </mdb-card>
            <mdb-modal centered :show="showModal2" @close="showModal2 = false">
              <mdb-modal-header>
                <mdb-modal-title>Durante el proceso</mdb-modal-title>
              </mdb-modal-header>
              <mdb-modal-body>
                <img style="width: 100%;" src="../../build/img/img-Marie/marie stopes landing-02.jpg">
              </mdb-modal-body>
              <mdb-modal-footer>
                <mdb-btn color="#FF0000" @click.native="showModal2 = false">Close</mdb-btn>
              </mdb-modal-footer>
            </mdb-modal>
          </mdb-col>
          <mdb-col md="4" class="mb-5">
            <mdb-card v-animateOnScroll="{animation: 'fadeInRight', delay: 400}"> 
              <mdb-btn class="buttom-process" color="#FF0000" @click.native="showModal3 = true">
                <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="50" height="50" viewBox="0 0 172 172" style=" fill:#000000; padding-bottom: 5px;">
                  <g fill="none" fill-rule="nonzero" stroke="none" stroke-width="1" stroke-linecap="butt" stroke-linejoin="miter" stroke-miterlimit="10" stroke-dasharray="" stroke-dashoffset="0" font-family="none" font-weight="none" font-size="none" text-anchor="none" style="mix-blend-mode: normal">
                    <path d="M0,172v-172h172v172z" fill="none">
                    </path>
                    <g fill="#ffffff">
                      <g id="surface1">
                        <path d="M86,6.88c-43.65844,0 -79.12,35.46156 -79.12,79.12c0,43.65844 35.46156,79.12 79.12,79.12c43.65844,0 79.12,-35.46156 79.12,-79.12c0,-43.65844 -35.46156,-79.12 -79.12,-79.12zM86,13.76c39.93625,0 72.24,32.30375 72.24,72.24c0,39.93625 -32.30375,72.24 -72.24,72.24c-39.93625,0 -72.24,-32.30375 -72.24,-72.24c0,-39.93625 32.30375,-72.24 72.24,-72.24zM75.3575,48.0525c-0.14781,0.02688 -0.29562,0.06719 -0.43,0.1075c-1.29,0.22844 -2.32469,1.16906 -2.6875,2.41875c-0.36281,1.26313 0.01344,2.60688 0.9675,3.49375l31.9275,31.9275l-31.9275,31.9275c-1.37062,1.37063 -1.37062,3.57438 0,4.945c1.37063,1.37063 3.57438,1.37063 4.945,0l34.4,-34.4c0.67188,-0.645 1.04813,-1.54531 1.04813,-2.4725c0,-0.92719 -0.37625,-1.8275 -1.04813,-2.4725l-34.4,-34.4c-0.71219,-0.76594 -1.74687,-1.15562 -2.795,-1.075z">
                        </path>
                      </g>
                    </g>
                  </g>
                </svg>
                <br>
                Después del proceso
              </mdb-btn>
            </mdb-card>
            <mdb-modal centered :show="showModal3" @close="showModal3 = false">
              <mdb-modal-header>
                <mdb-modal-title>Antes del proceso</mdb-modal-title>
              </mdb-modal-header>
              <mdb-modal-body>
                <img style="width: 100%;" src="../../build/img/img-Marie/marie stopes landing-04.jpg">
              </mdb-modal-body>
              <mdb-modal-footer>
                <mdb-btn color="#FF0000" @click.native="showModal3 = false">Cerrar</mdb-btn>
              </mdb-modal-footer>
            </mdb-modal>
          </mdb-col>
        </mdb-row>
        <mdb-row>
          <!-- INICIA CALCILADORA -->
          <h2 class="font-weight-bold fl-porto mt-5 calculadora-titulo" ref="calculadora-ref" style="width: 100%;">Calcula tu Tiempo de Embarazo</h2>
          <mdb-col md="7" class="mb-5">
            <p style="font-size: 14px;">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. </p>
            <select class="calculator" v-model="selectedDay">
              <option value="">Día</option>
              <option v-for="option in optionsDays" v-bind:key="option.value">{{option.text}}</option>
            </select>
            <select class="calculator" v-model="selectedMonth">
                <option value="">Mes</option>
                <option v-for="option in optionsMonth" v-bind:key="option.valor">{{option.valor}}</option>
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
              <strong style="color: #00B3E8; font-size: 30px; font-weight: bold;">{{Results}}</strong><br>
            </mdb-card-text>
          </mdb-col>
          <mdb-col md="5" class="mb-5">
            <img style="width: 80%;" src="../../build/img/img-Marie/marie stopes landing-05.jpg">
          </mdb-col>
        </mdb-row>
        
        <h2 class="text-center mt-5 font-weight-bold fl-porto" ref="quest">PREGUNTAS FRECUENTES</h2>
        <mdb-col md="8" class="mx-auto text-center mb-5" style="font-size: 15px;">
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
        </mdb-col>
        <mdb-accordion :panes="panes"/>
      </mdb-container>
    </div>
    <mdb-footer class="footer-section">
      <p class="footer-copyright mb-0 py-3 text-center">
        Términos y condiciones de uso  
        <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="10" height="10" viewBox="0 0 172 172" style=" fill:#000000; margin-bottom: 2px; padding: 2px;">
          <g fill="none" fill-rule="nonzero" stroke="none" stroke-width="1" stroke-linecap="butt" stroke-linejoin="miter" stroke-miterlimit="10" stroke-dasharray="" stroke-dashoffset="0" font-family="none" font-weight="none" font-size="none" text-anchor="none" style="mix-blend-mode: normal">
            <path d="M0,172v-172h172v172z" fill="none">
            </path>
            <g fill="#ffffff">
              <path d="M86,165.12c-43.62952,0 -79.12,-35.49392 -79.12,-79.12c0,-43.62608 35.49048,-79.12 79.12,-79.12c43.62952,0 79.12,35.49392 79.12,79.12c0,43.62608 -35.49048,79.12 -79.12,79.12z">
              </path>
            </g>
          </g>
        </svg>
         Politicas de privacidad
      </p>
    </mdb-footer>
  </div>
</template>

<script>
import { mdbContainer, mdbModal, mdbModalHeader, mdbModalTitle, mdbModalBody, mdbModalFooter, mdbCol, mdbRow, mdbIcon, mdbNavbarBrand, mdbNavbar, mdbNavItem, mdbNavbarNav, mdbNavbarToggler, mdbBtn, mdbEdgeHeader, mdbFooter, mdbCard, mdbCardImage, mdbCardTitle, mdbCardText, mdbCardBody, animateOnScroll, mdbAccordion} from 'mdbvue';
import moment from 'moment';

export default {
  name: 'HomePage',
  components: {
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
      panes: [
        {
          title: 'Collapsible Group Item #1',
          content: 'Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven\'t heard of them accusamus labore sustainable.'
        }, {
          title: 'Collapsible Group Item #2',
          content: 'Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven\'t heard of them accusamus labore sustainable.'
        },
        {
          title: 'Collapsible #FF0000Group Item #3',
          content: 'Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven\'t heard of them accusamus labore sustainable.'
        }
      ]
    };
  },
  directives: {
    animateOnScroll
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
    scrollMeTo(refName) {
      var element = this.$refs[refName];
      var top = element.offsetTop;
      window.scrollTo(0, top);
    },
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
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
  background: url('../../build/img/img-Marie/fondo.jpg') center;
  background-size: cover;
}
.header-logo-navbar{
  max-width: 200px;
  width: 100%;
}

.send-buttom{
  width: 100%; 
  background: #00C5FF; 
  border-radius: 6px 6px 6px 6px;
  -moz-border-radius: 6px 6px 6px 6px;
  -webkit-border-radius: 6px 6px 6px 6px;
  border: 0px solid #000000;
  font-size: 20px;
  color: white;
  font-weight: bold;
  padding: 5px;
}
.demo-section{
  width: 50%;
  height: 80%;
  background: #000000;
}

.whats-icon{
  width: 100%;
  margin-top: 25px;
}

.phone-number{
  color: white;
  font-weight: bold;
  font-size: 22px;
  margin: 75px 0px 0px 70px;
}

.input-secction{
    display: block;
    top: 165px;
    width: 325px;
    background-color: rgba(0,0,0,.5);;
    padding: 30px;
    height: 505px;
    margin-right: 100px;
}

.buttom-process{
  background: #FF0000;
  border: 0px;
  height: 100px;
  border-radius: 6px 6px 6px 6px;
  -moz-border-radius: 6px 6px 6px 6px;
  -webkit-border-radius: 6px 6px 6px 6px;
  color: white;
  font-weight: bold;
}

.calculator{
  background: white;
  padding: 10px 30px 10px 10px;
  border-radius: 6px 6px 6px 6px;
  -moz-border-radius: 6px 6px 6px 6px;
  -webkit-border-radius: 6px 6px 6px 6px;
}

.calculato-buttom{
  width: 15%; 
  background: #00B3E8; 
  border-radius: 6px 6px 6px 6px;
  -moz-border-radius: 6px 6px 6px 6px;
  -webkit-border-radius: 6px 6px 6px 6px;
  border: 0px solid #000000;
  font-size: 15px;
  color: white;
  font-weight: bold;
  padding: 10px;
}

.buttom-question{
  background: white;
  border: 0px;
  height: 40px;
  border-radius: 6px 6px 6px 6px;
  -moz-border-radius: 6px 6px 6px 6px;
  -webkit-border-radius: 6px 6px 6px 6px;
  font-weight: bold;
}

.buttom-question:hover{
  background: #FF0000;
  color: white;
}

.buttom-question:active{
  background: #FF0000;
  color: white;
}

.form-section{
  border: #000000;
}

.send-buttom2{
  width: 20%; 
  background: #00C5FF; 
  border-radius: 6px 6px 6px 6px;
  -moz-border-radius: 6px 6px 6px 6px;
  -webkit-border-radius: 6px 6px 6px 6px;
  border: 0px solid #000000;
  font-size: 20px;
  color: white;
  font-weight: bold;
  padding: 5px;
}

.form-extra{
  padding: 0% 0% 20% 1%;;
}

.blue-bar-title{
  color: white;
  padding: 25px 0px 0px 50px;
  font-weight: bold;
}

.blue-bar-subtitle{
  color: white; 
  padding: 0px 0px 0px 50px; 
  font-size: 15px;
}

.card-text-content{
  height: 220px;
}

.porto-button{
  margin-right: 10px;
}

.footer-section{
  background: #1f1e1e;
  color: white;
}

@media (max-width: 767px) {
  .input-secction{
    width: 100%;
    top: 80px;
    padding: 50px;
  }
  .blue-bar{
    height: 575px;
    padding-top: 40px;
    text-align: center;
  }
  .blue-bar-title{
    padding: 10px 0px 0px 0px;
    font-size: 25px;
  }
  .blue-bar-subtitle{
    padding: 5px 0px 0px 0px;
    font-size: 10px;
  }
  .calculato-buttom{
    width: 100%;
    margin-top: 10px;
  }
  .card-text-content{
    height: 300px;
  }
  .card-text-content-extra{
    height: 350px;
  }
  .calculadora-titulo{
    padding-left: 15px;
  }
  .footer-section{
  background: #1f1e1e;
  color: white;
  }
}

@media (max-width: 1024px) {
  .input-secction{
    width: 100%;
    height: 71%;
    top: 120px;
    padding-top: 10px; 
    margin-right: 30px;
  }
  .blue-bar{
    height: 575px;
    padding-top: 40px;
    text-align: center;
  }
  .blue-bar-title{
    padding: 15px 0px 0px 0px;
  }
  .blue-bar-subtitle{
    padding: 0px;
  }
  .calculato-buttom{
    width: 100%;
    margin-top: 10px;
  }
  .card-text-content{
    height: 300px;
  }
  .card-text-content-extra{
    height: 350px;
  }
  .calculadora-titulo{
    padding-left: 15px;
  }
  .footer-section{
  background: #1f1e1e;
  color: white;
  }
  .phone-number{
    font-size: 45px;
    margin: 30px 0px 0px 10px;
  }
}

</style>
