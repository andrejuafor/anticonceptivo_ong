<template>
    <div style="margin-top: -60px;">
<!----------------------------------------------------------------------------------------------------------------->
      <mdb-edge-header style="height: 590px;">
        <div class="home-page-background">
          <mdb-col class="input-secction" sm="6">
            <section class="demo-section ">
              <section>
                <p style="color: #FFFFFF; font-weight: bold; font-size: 20px;">Contáctanos</p>
                <p>Lorem ipsum el dolore sit amet</p>
                <div>
                  <input class="form-control" type="text" placeholder="Nombre"/>
                  <br/>
                  <input class="form-control" type="text" placeholder="Teléfono"/>
                  <br/>
                  <input class="form-control" type="text" placeholder="Correo electrónico"/>
                  <br/>
                  <input class="form-control form-control-lg" type="text" placeholder="Mensaje (máximo 250 caracteres)"/>
                  <br/>
                  <button class="send-buttom">Enviar</button>
                </div>
              </section>
            </section>
          </mdb-col>
        </div>
      </mdb-edge-header>
<!----------------------------------------------------------------------------------------------------------------->
      <mdb-container>
        <h2 class="text-center mt-5 font-weight-bold">EL PROCESO</h2>
        <mdb-col md="10" class="mx-auto text-center text-muted mb-5">
          <p>Antes de iniciar el proceso, considera lo siguiente</p>
        </mdb-col>
<!----------------------------------------------------------------------------------------------------------------->
        <mdb-row>
          <mdb-col md="4" class="mb-5">
            <mdb-card class="animated fadeInLeft">
              <mdb-card-body>
                <mdb-card-title><mdb-icon fab icon="css3" class="pink-text" /><strong>CONFIRMA QUE ESTAS EMBARAZADA</strong></mdb-card-title>
                <mdb-card-text>Poniendo atención a los síntomas puedes hacer una comparación después de haber usado las pastillas. <br/><br/> Puedes confirmar con una prueba de orina de farmacia. 
                Para mayor certeza y oara conocer la edad gestional. puedes realizar un ultrasonido.</mdb-card-text>
              </mdb-card-body>
            </mdb-card>
          </mdb-col>
          <mdb-col md="4" class="mb-5">
            <mdb-card class="animated fadeInRight">
              <mdb-card-body>
                <mdb-card-title><mdb-icon fab icon="code" class="green-text" /><strong>ASEGÚRATE DE QUE EL EMBARAZO ESTÁ DENTRO DEL ÚTERO</strong></mdb-card-title>
                <mdb-card-text>Si además sientes dolor intenso que se concentra en un lado (bajo vientre derecho o izquierdo), 
                  que se presenta de repente, con palpitaciones y debilidad <strong>¡requieres atención médica urgente y no puedes iniciar el proceso!</strong></mdb-card-text>
              </mdb-card-body>
            </mdb-card>
          </mdb-col>
        </mdb-row>
<!----------------------------------------------------------------------------------------------------------------->
        <mdb-row>
          <mdb-col md="4" class="mb-5">
            <mdb-card class="animated fadeInLeft" >
              <mdb-card-body>
                <mdb-card-title><mdb-icon fab icon="css3" class="pink-text" /><strong>LA EDAD GESTIONAL</strong></mdb-card-title>
                <mdb-card-text>¿Cuantas semanas de embarazo tienes?<br><br>Puedes calcularlo de la siguiente forma: contar los dias desde el primer día de la decha de la última menstrución,
                el resultado en días divídelo entre 7 para conocer las semanas. Si es posible, confima con ulrasonido</mdb-card-text>
              </mdb-card-body>
            </mdb-card>
          </mdb-col>
          <mdb-col md="4" class="mb-5">
            <mdb-card class="animated fadeInRight">
              <mdb-card-body>
                <mdb-card-title><mdb-icon fab icon="code" class="green-text" /><strong>IMPORTANTE</strong></mdb-card-title>
                <mdb-card-text><strong>¿Tienes colocado algún dispositivo intrauterino (DIU o SIU)?</strong><br>
                En caso de tener alguno, debes retirarlo antes de tomar las pastillas. <br>
                <strong>¿Eres alérgica a la mifepristona o al misoprostol?</strong><br>
                Si eres alérgica, no las tomes y considera otra opcion para tu interrupcion. <br>
                <strong>¿Tienes problemas de coagulación, padeces anemia severa, asma no controlada o usas corticoides?</strong><br>
                Para iniciar el proceso con las pastillas rquieres vigilancia médica.<br>
                </mdb-card-text>
              </mdb-card-body>
            </mdb-card>
          </mdb-col>
        </mdb-row>
<!----------------------------------------------------------------------------------------------------------------->
        <mdb-row>
          <mdb-col md="4" class="mb-5">
            <mdb-card v-animateOnScroll="{animation: 'fadeInLeft', delay: 400}">
              <mdb-card-image src="https://mdbootstrap.com/wp-content/uploads/2017/06/navigation-1.jpg" alt="Card image cap"></mdb-card-image>
              <mdb-card-body>
                <mdb-card-title><mdb-icon icon="bars" class="pink-text" /><strong> NAVIGATION</strong></mdb-card-title>
                <mdb-card-text>Ready-to-use navigation layouts, navbars, breadcrumbs and much more! More about our navigation components.</mdb-card-text>
                <mdb-nav-item to="/navigation" class="float-right" anchorClass="p-0"><mdb-btn color="elegant">More</mdb-btn></mdb-nav-item>
              </mdb-card-body>
            </mdb-card>
          </mdb-col>
          <mdb-col md="4" class="mb-5">
            <mdb-card v-animateOnScroll="{animation: 'fadeIn'}">
              <mdb-card-image src="https://mdbootstrap.com/wp-content/uploads/2015/08/forms.jpg" alt="Card image cap"></mdb-card-image>
              <mdb-card-body>
                <mdb-card-title><mdb-icon icon="edit" class="blue-text" /><strong> FORMS</strong></mdb-card-title>
                <mdb-card-text>Inputs, autocomplete, selecst, date and time pickers. Everything in one place is ready to use!</mdb-card-text>
                <mdb-nav-item to="/forms" class="float-right" anchorClass="p-0"><mdb-btn color="elegant">More</mdb-btn></mdb-nav-item>
              </mdb-card-body>
            </mdb-card>
          </mdb-col>
          <mdb-col md="4" class="mb-5">
            <mdb-card v-animateOnScroll="{animation: 'fadeInRight', delay: 200}">
              <mdb-card-image src="https://mdbootstrap.com/wp-content/uploads/2015/08/table-fb.jpg" alt="Card image cap"></mdb-card-image>
              <mdb-card-body>
                <mdb-card-title><mdb-icon icon="table" class="green-text" /><strong> TABLES</strong></mdb-card-title>
                <mdb-card-text>Basic and advanced tables. Responsive, datatables, with sorting, searching and export to csv.</mdb-card-text>
                <mdb-nav-item to="/tables" class="float-right" anchorClass="p-0"><mdb-btn color="elegant">More</mdb-btn></mdb-nav-item>
              </mdb-card-body>
            </mdb-card>
          </mdb-col>
        </mdb-row>
        <mdb-row class="mb-4">
          <mdb-col md="4" class="mb-5">
            <mdb-card v-animateOnScroll="{animation: 'fadeInLeft', delay: 400}">
              <mdb-card-image src="https://mdbootstrap.com/wp-content/uploads/2018/02/modal-new.jpg" alt="Card image cap"></mdb-card-image>
              <mdb-card-body>
                <mdb-card-title><mdb-icon icon="window-restore" class="pink-text" /><strong> MODALS</strong></mdb-card-title>
                <mdb-card-text>Modals are great for displaying advanced messages to the user. Cookies, logging in, registration and much more.</mdb-card-text>
                <mdb-nav-item to="/modals" class="float-right" anchorClass="p-0"><mdb-btn color="elegant">More</mdb-btn></mdb-nav-item>
              </mdb-card-body>
            </mdb-card>
          </mdb-col>
          <mdb-col md="4" class="mb-5">
            <mdb-card v-animateOnScroll="{animation: 'fadeIn'}">
              <mdb-card-image src="https://mdbootstrap.com/img/Marketing/docs/social/main-addons.jpg" alt="Card image cap"></mdb-card-image>
              <mdb-card-body>
                <mdb-card-title><mdb-icon icon="plus-square" class="blue-text" /><strong> PLUGINS & ADDONS</strong></mdb-card-title>
                <mdb-card-text>Find out more about our extended components.</mdb-card-text>
                <mdb-nav-item to="/plugins" class="float-right" anchorClass="p-0"><mdb-btn color="elegant">More</mdb-btn></mdb-nav-item>
              </mdb-card-body>
            </mdb-card>
          </mdb-col>
        </mdb-row>
      </mdb-container>
    </div>
</template>

<script>
import { mdbContainer, mdbCol, mdbRow, mdbIcon, mdbNavbar, mdbNavItem, mdbNavbarNav, mdbNavbarToggler, mdbBtn, mdbEdgeHeader, mdbCard, mdbCardImage, mdbCardTitle, mdbCardText, mdbCardBody, animateOnScroll } from 'mdbvue';

export default {
  name: 'HomePage',
  components: {
    mdbContainer,
    mdbCol,
    mdbRow,
    mdbIcon,
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
    mdbCardBody
  },
  directives: {
    animateOnScroll
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
  background: url('https://www.turismodeobservacion.com/media/fotografias/atardecer-en-cortegana-3123-xl.jpg') center;
  background-size: cover;
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

.input-secction{
  display: block;
  top: 132px;
  left: 850px;
}

</style>
