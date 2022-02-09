<script>
    import Footer from "./partials/Footer.svelte";
    import Nav from "./partials/Nav.svelte";
</script>

<link rel="stylesheet" href="css/marketing.css" />
<Nav />

<section class="bloque1 pt-5 text-white">
    <!-- particles.js container -->
    <div id="particles-js" />
    <div class="container">
        <div class="row">
            <div class="col-sm my-auto">
                <div class="">
                    <div class="titulo-negocioremesas">
                        <h1 class="text-center titulo">
                            <strong>Aprende sobre Criptomonedas</strong>
                        </h1>
                        <div class="animacion  text-center ">
                            <ul>
                                <li>ANALISIS.</li>
                                <li>EXCHANGE.</li>
                                <li>DIVERSIFICAR.</li>
                            </ul>
                        </div>
                        <div class="container" style="font-size: 1.8rem;">
                            <p class="">
                                Con este curso completo de trading lograras
                                aprender cómo invertir en criptomonedas, ya seas
                                principiante o quieras ampliar tus
                                conocimientos.
                            </p>
                            <br />
                            <p class="">
                                Acompañado por un asesor tendrás la oportunidad
                                de consultar todas las dudas sobre cualquier
                                modulo, ya que brindamos asesoría ilimitada y
                                personalizada para todos nuestros alumnos. Como
                                parte de nuestro método de enseñanza buscamos
                                que nuestros alumnos tengan como pilar
                                fundamental la disciplina, ser cautelosos para
                                no operar con emociones y hacer una buena
                                gestión.
                            </p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-sm">
                <div class="flex2 d-flex justify-content-center">
                    <img
                        src="img/43.png"
                        alt=""
                        class="img-fluid"
                        style="min-width:300px"
                    />
                </div>
            </div>
        </div>
    </div>
</section>

<!-- DESCRIPCION DE NIVELES  -->

<div class="container-fluid bg-dark pt-5">
    <div class="container">
        <div class="text-center text-white py-2">
            <h2 class="mt-1 oferta3">Nuestros Niveles de Capacitacion</h2>
        </div>

        <div class="row">
            <div class="col-lg-4 col-md-6 col-sm-12 ">
                <div class="card mb-5 shadow-sm ">
                    <img
                        src="img/tradinglvl1.jpg"
                        alt=""
                        class="img-fluid"
                        style="height: 280px;"
                    />

                    <div class="card-body">
                        <div class="card-title">
                            <h4 class="letra">¡Análisis del Mercado!</h4>
                        </div>
                        <div class="card-text" style="font-size: 1.5rem;">
                            <p>
                                Aprenderás técnicas para analizar los gráficos,
                                acción del precio, temporalidades y mucho más.
                                Serás capaz de entender el movimiento del
                                mercado y gestionar tus propios análisis
                                técnicos con la guía de tu asesor.
                            </p>
                        </div>
                        <a
                            href="/trading/nivel1"
                            class="btn btn-outline-primary rounded-0 float-end "
                            style="font-size: 1.8rem;">Leer más</a
                        >
                    </div>
                </div>
            </div>

            <div class="col-lg-4 col-md-6 col-sm-12 ">
                <div class="card mb-5 shadow-sm">
                    <img
                        src="img/tradinglvl2.jpg"
                        alt=""
                        class="img-fluid"
                        style="height: 280px;"
                    />

                    <div class="card-body">
                        <div class="card-title">
                            <h4 class="letra">¡Invierte en Criptos!</h4>
                        </div>
                        <div class="card-text" style="font-size: 1.5rem;">
                            <p>
                                En este segundo nivel aprenderás a operar en el
                                Exchange y diferente billeteras. Lograras
                                convertir tu capital en USDT, abrir y cerrar
                                operaciones, ordenes, margen y mucho más
                                apuntando en diferentes mercados.
                            </p>
                        </div>
                        <a
                            href="/trading/nivel2"
                            class="btn btn-outline-primary rounded-0 float-end"
                            style="font-size: 1.8rem;">Leer más</a
                        >
                    </div>
                </div>
            </div>

            <div class="col-lg-4 col-md-6 col-sm-12">
                <div class="card mb-5 shadow-sm">
                    <img
                        src="img/tradinglvl3.jpg"
                        alt=""
                        class="img-fluid"
                        style="height: 280px;"
                    />

                    <div class="card-body">
                        <div class="card-title">
                            <h4 class="letra">¡Distribuye!</h4>
                        </div>
                        <div class="card-text " style="font-size: 1.5rem;">
                            <p>
                                En este tercer nivel aprenderás a diversificar
                                tu capital y resguardar tu liquidez para así
                                reducir los riesgos y aumentar tus ganancias. Te
                                recomendaremos con cuanto porcentaje debes abrir
                                las operaciones.
                            </p>
                        </div>
                        <a
                            href="/trading/nivel3"
                            class="btn btn-outline-primary rounded-0 float-end"
                            style="font-size: 1.8rem;">Leer más</a
                        >
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

<div class="container-fluid bg-white px-0 border-0">
    <div clss="bg-black">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"
            ><path
                fill="#00000"
                fill-opacity="1"
                d="M0,288L60,293.3C120,299,240,309,360,288C480,267,600,213,720,186.7C840,160,960,160,1080,176C1200,192,1320,224,1380,240L1440,256L1440,0L1380,0C1320,0,1200,0,1080,0C960,0,840,0,720,0C600,0,480,0,360,0C240,0,120,0,60,0L0,0Z"
            /></svg
        >
    </div>

    <div class="container pb-5">
        <div class="row mx-1 ">
            <div class="col-lg-6 ">
                <h2 class=" oferta"><strong>OFERTA </strong></h2>
                <h2 class=" oferta"><strong>EXCLUSIVA</strong></h2>
                <br />

                <div id="cuenta" class="mb-3" />

                <h3
                    class="  oferta35 text-danger  "
                    style="line-height:6.5rem;"
                >
                    40%
                </h3>

                <h4 class=" text-danger oferta3">de descuento</h4>
                <h3 class="letra">Accede al paquete completo</h3>
                <ul>
                    <li class="letra2">
                        <i class="fas fa-angle-right" /> Acceso a los niveles del
                        curso.
                    </li>
                    <li class="letra2">
                        <i class="fas fa-angle-right" /> Asesoria ilimitada.
                    </li>
                    <li class="letra2">
                        <i class="fas fa-angle-right" /> Acceso gratuito a las actualizaciones.
                    </li>
                    <li class="letra2">
                        <i class="fas fa-angle-right" /> Membresia por 30 dias al
                        grupo de señales.
                    </li>
                </ul>

                <h4 class="letra">Antes<s> 140 USD</s></h4>
                <h2 class="oferta3"><strong>Ahora 99.99 USD</strong></h2>
                <a
                    href="/oferta"
                    class="btn btn-danger"
                    style="font-size: 2rem;">Quiero la Oferta</a
                >
            </div>
            <div class="col-lg-6">
                <img
                    src="img/oferta.png"
                    alt=""
                    class="img-fluid mx-auto my-3"
                />
                <div class="text-center">
                    <a
                        href="https://wa.me/message/TPZZ36SKBAC5J1"
                        target="_blank"
                        class="btn btn-success text-center p-3"
                        style="font-size: 2rem;"
                        ><i class="fab fa-whatsapp" /> Contactar por Whatsapp</a
                    >
                </div>
            </div>
        </div>
    </div>
</div>
<Footer />
