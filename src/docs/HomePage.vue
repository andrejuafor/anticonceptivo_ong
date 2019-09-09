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
            <p class="h5 contact-title" style="color: white;">Contáctanos</p>
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
                <p>
                  <strong>INTERRUPCIÓN SEGURA DEL EMBARAZO CON PASTILLAS</strong>
                  <br><br>
                  <strong>¿Sabías qué..?</strong>
                  <br><br>
                  El aborto con pastillas es un proceso. Al ser casi idéntico al aborto espontaneo, es más natural y menos invasivo. No se trata de un procedimiento, la finalidad de este proceso es interrumpir el embarazo y no vaciar el útero al momento de usar las pastillas, el útero se irá vaciando al paso de los días.
                  <br><br>
                  <strong>Además…</strong>
                  <br><br>
                  La Organización Mundial de la Salud dice que usar las pastillas en casa, es una opción segura para las mujeres que necesitan interrumpir su embarazo.
                  <br><br>
                  <strong>Tratamiento de mifepristona + misoprostol:</strong>
                  <br>
                  El uso combinado de los medicamentos hará tu proceso más rápido, más eficaz y con menos efectos secundarios.
                  <br><br>
                  <strong>Sobre las pastillas……</strong>
                  <br><br>
                  <strong>¿Por qué son dos medicamentos 1 pastilla de mifepristona y sólo 4 pastillas de misoprostol?</strong>
                  <br><br>
                  La mifepristona potencializa los efectos del misoprostol y hace el proceso 3 veces más efectivo. Por lo tanto, necesitas 1 pastilla de mifepristona y solo 4 pastillas de misoprostol para iniciar tu proceso de interrupción.
                  <br><br>
                  <strong>¿Cómo saber que las pastillas están en buenas condiciones?</strong>
                  <br>
                  Revisa lo siguiente:
                  <li>
                    <ul><mdb-icon icon="circle" class="fa-xs"/> Que la fecha de caducidad sea menor a 2 años.</ul>
                    <ul><mdb-icon icon="circle" class="fa-xs"/> Que la caja se encuentre cerrada</ul>
                    <ul><mdb-icon icon="circle" class="fa-xs"/> Que el empaque (la lámina de aluminio en la que se encuentran encapsuladas las pastillas) cubra por ambos lados cada tableta.</ul>
                    <ul><mdb-icon icon="circle" class="fa-xs"/> Que estén en un lugar fresco.</ul>
                  </li>                                           
                  <br><br>
                  <strong>¿Qué tan efectiva es esta opción?</strong>
                  <br>
                  El uso combinado de MIFEPRISTONA + MISOPROSTOL es el tratamiento reconocido por la Organización Mundial de la Salud como el “estándar de oro” por el alto porcentaje de efectividad que tiene para que las mujeres puedan interrumpir su embarazo de forma segura. La probabilidad de falla del tratamiento combinado (mife + miso) es de 5 en 100, mientras que la de misoprostol solo es de 15 en 100.
                </p>
                <!-- <img style="width: 100%;" src="../../build/img/img-Marie/marie stopes landing-03.jpg"> -->
              </mdb-modal-body>
              <mdb-modal-footer>
                <mdb-btn color="green">Descargar</mdb-btn>
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
                <mdb-modal-title>ANTES DEL PROCESO</mdb-modal-title>
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
                    <ul><mdb-icon icon="circle" class="fa-xs"/> Retraso del periodo menstrual</ul>
                    <ul><mdb-icon icon="circle" class="fa-xs"/> Mayor sensibilidad en los senos</ul>
                    <ul><mdb-icon icon="circle" class="fa-xs"/> Náuseas y/o vómito, especialmente al despertar </ul>
                    <ul><mdb-icon icon="circle" class="fa-xs"/> Dolor de cabeza</ul>
                    <ul><mdb-icon icon="circle" class="fa-xs"/> Cansancio</ul>
                    <ul><mdb-icon icon="circle" class="fa-xs"/> Orinar con mucha frecuencia</ul>
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
                </p>
                <!-- <img style="width: 100%;" src="../../build/img/img-Marie/marie stopes landing-03.jpg"> -->
              </mdb-modal-body>
              <mdb-modal-footer>
                <mdb-btn color="green">Descargar</mdb-btn>
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
                <p>
                  <strong>Durante el proceso:</strong> 
                  <br><br>
                  <strong>¿Cómo tomar las pastillas?</strong>
                  <br><br>
                  Tragar una pastilla de MIFEPRISTONA con agua, esta pastilla no produce molestia, pero puede llegar a aparecer un leve sangrado
                  <br><br>
                  Una hora antes de colocar el misoprostol, traga con agua 2 pastillas de IBUPROFENO de 400mg.
                  <br><br>
                  El ibuprofeno ayudará a reducir las molestias que pudieran presentarse con el misoprostol, síguelo tomando por 5 días cada 8 horas. El ibuprofeno no afecta el proceso de interrupción, sólo ayuda a disminuir la molestia, es importante que lo tomes con mínimo una hora de anticipación para que pueda absorberse y su efecto analgésico comience antes de que se presenten las molestias.
                  <br><br>
                  En un lapso de 24 a 48 hrs después de tomar la mifepristona, coloca 4 pastillas de MISOPROSTOL, dos entre el cachete y la encía superior derecha y dos entre el cachete y la encía superior izquierda, deja pasar 30 minutos.
                  <br><br>
                  Puedes pasar la saliva de forma normal pero sin tragar las pastillas. Cuando pasen los 30 minutos, si aún quedan restos de las pastillas, puedes pasarlos con agua.
                  <br><br>
                  <strong>¿Qué voy a sentir?</strong> 
                  <br><br>
                  A partir de la primera media hora presentarás sangrado y cólico. Puede que también se presenten: escalofríos, mareo, náuseas, vómito, diarrea, y/o fiebre pasajera. Estos últimos no se presentan siempre, y puede o no que aparezcan, pero en caso de que los llegaras a experimentar no debes alarmarte, son pasajeros y se quitan solos por completo. No es necesario tomar otro medicamento.
                  <br><br>
                  <strong>¿Qué tanto duele?</strong>
                  <br><br>
                  El cuerpo de cada mujer es diferente, por lo que, al igual que el sangrado, no existe una intensidad definida para el dolor. El ibuprofeno ayudará a controlar las molestias. También puedes ayudarte de compresas calientes en el vientre y espalda baja.
                  <br><br>
                  <strong>¿Qué tanto tengo que sangrar?</strong>
                  <br><br>
                  Las primeras horas después de haber colocado el misoprostol se presentará la mayor cantidad de sangrado, pero no hay una cantidad definida. Puede durar como un periodo menstrual o extenderse hasta 30 días con tendencia a disminuir. Recuerda que el sangrado nunca debe ser mayor a empapar 2 toallas regulares en 1 hora por 2 horas seguidas. El sangrado puede llegar a ser intermitente, es decir, que unos días haya y otros días no. También puede cambiar de color: ser rosa, marrón o café
                  <br><br>
                  <strong>¿Cuándo debo preocuparme?</strong>
                  <br><br> 
                  <li>
                    <ul>- Sangrado mayor a empapar 2 toallas regulares en 1 hora por 2 horas seguidas</ul>
                    <ul>- Coágulos más grandes que un limón</ul>
                    <ul>- Fiebre que persiste por más de 24 horas </ul>
                    <ul>- Si 48 hrs. después de haber colocado el misoprostol no hay sangrado.</ul>
                  </li>
                  <br><br>
                  Si presentas alguna de estas señales, acude con alguna proveedora de salud para que seas valorada 
                  <br><br>
                  <strong>¿Puedo comer de todo?</strong>
                  <br><br>
                  Tu alimentación puede continuar de manera normal, como cuando estás menstruando. Hazle caso a tu cuerpo, si tienes hambre o se te antoja algo, puedes comerlo, eso no alterará el efecto de las pastillas.
                </p>
              </mdb-modal-body>
              <mdb-modal-footer>
                <mdb-btn color="green">Descargar</mdb-btn>
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
                <mdb-modal-title>Antes del proceso</mdb-modal-title>
              </mdb-modal-header>
              <mdb-modal-body>
                <p>
                  <strong>DESPUÉS DEL PROCESO</strong>
                  <br><br>
                  <strong>Lo más frecuente…</strong>
                  <br>
                  es que la expulsión ocurra en las primeras 4 horas, sin embargo se trata de un proceso en el que el útero se irá limpiando con el paso de los días , es por esta razón que el sangrado puede extenderse de 14 hasta 30 días, aproximadamente. También es importante que recuerdes cómo te sentías antes de tomar las pastillas, piensa en los síntomas que se han ido días después de usarlas.
                  <br><br>
                  Por ejemplo:
                  <li>
                    <ul>- Ausencia de sangrado (esto es lo primero que notarás diferente).</ul>
                    <ul>- Dolor de senos</ul>
                    <ul>- Náuseas y/o vómito </ul>
                    <ul>- Dolor de Cabeza</ul>
                    <ul>- Cansancio y/o sueño</ul>
                  </li>
                  <br><br>
                  - A los 5 días de haber usado las pastillas, notarás que estos síntomas van desapareciendo.
                  <br><br>
                  <strong>Después de 14 días…</strong>
                  <br><br>
                  Con ayuda de la prueba de embarazo, podrás confirmar la interrupción, pero si te sientes más tranquila, puedes corroborar con ultrasonido.
                  <br><br>
                  <strong>¿Cómo usar prueba de orina?</strong> 
                  <li>
                    <ul>1. Coloca un poco de orina en un recipiente desechable</ul>
                    <ul>2. Una vez abierta tu prueba, sujeta con tus dedos el extremo  de color y no toques el extremo blanco.</ul>
                    <ul>3. Sumerge en la orina el extremo blanco hasta la línea de color durante un minuto</ul>
                    <ul>4. Retira la prueba de la orina y espera un minuto mientras arroja el resultado</ul>
                  </li>
                  <br><br>
                  <strong>Resultado</strong>
                  <br>
                  Si solo aparece una línea, tu prueba es <strong>negativa</strong>
                  <br>
                  Si observas <strong>dos líneas</strong>, el resultado es <strong>positivo</strong>. En caso de que sea positivo, comprueba con un ultrasonido. Si el resultado definitivo es positivo, es necesario evaluar una segunda dosis de medicamento o hacer un procedimiento de aspiración.
                  <br><br>
                  <strong>¡DATOS DE ALARMA!</strong>
                  <br>
                  <li>
                    <ul>- Continuación del embarazo.</ul>
                    <ul>- Presencia de alguna infección</ul>
                    <ul>- Sangrado mayor al esperado  </ul>
                  </li>
                  <br><br>
                  Debes saber que, en caso de que presentes alguna señal de alarma, es tu derecho solicitar atención médica. <strong>NO</strong> existe ningún examen clínico o sanguíneo que detecte el uso de las pastillas.
                  Las complicaciones que pudieran presentarse son consideradas como <strong>emergencia médica.</strong>
                  La regulación y leyes en materia de aborto obligan a los prestadores y  prestadoras de salud a atenderte. 
                </p>
              </mdb-modal-body>
              <mdb-modal-footer>
                <mdb-btn color="green">Descargar</mdb-btn>
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
import axios from 'axios';

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
      url:'http://localhost:8080/static/img/marie%20stopes%20landing-03.31fcfac.jpg',
      showModal: false,
      showModal2: false,
      showModal3: false,
      showModal4: false,
      panes: [
        {
          title: '<strong>¿Qué necesito para poder realizar mi aborto con pastillas)?</strong>',
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
    },
    forceFileDownload(response){
      const url = window.URL.createObjectURL(new Blob([response.data]));
      const link = document.createElement('a');
      link.href = url;
      link.setAttribute('download', 'file.png');
      document.body.appendChild(link);
      link.click();
    },
    downloadWithAxios(){
      axios({method: 'get', url: this.url, responseType: 'arraybuffer'}).then(response => {this.forceFileDownload(response);})
        .catch(() => console.log('error occured'));}
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
  width: 80%;
  margin: 20px 0px 5px 5px;
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
  margin: -18px;
}

.phone-number{
  color: white;
  font-weight: bold;
  font-size: 18px;
  margin-left: -15px;
}

.input-secction{
    display: block;
    top: 535px;
    width: 10%;
    height: 20%;
    background-color: rgba(0,0,0,.5);;
    padding: 30px;
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

@media (max-width: 766px) {
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
    height: 10%;
    top: 500px;
    padding-top: 50px; 
    margin-right: 30px;
  }
  .contact-title{
    margin: -40px 0px -10px -40px;
  }
  .whats-icon{
    width: 20%;
    margin: 12px 0px 5px -25px;
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
    font-size: 40px;
    margin: -63px 0px 0px 45px;
  }
}

</style>
