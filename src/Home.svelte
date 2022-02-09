<script>
    import Nav from "./partials/Nav.svelte";
    import Footer from "./partials/Footer.svelte";
    // for svg and page animation effect
    import { draw, fade, fly } from "svelte/transition";

    //viene lo de euro
    let coins = [];
    let btc = {};

    const loadCoins = async () => {
        const res = await fetch(
            "https://api.coingecko.com/api/v3/coins/markets?vs_currency=usd&order=market_cap_desc&per_page=100&page=1&sparkline=false"
        );
        const data = await res.json();
        coins = data;
        btc = coins[0].current_price.toLocaleString();
        console.log(btc);
    };
    loadCoins();
</script>

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
                                <li>SEÑALES</li>
                                <li>TRADING</li>
                                <li>REMESAS</li>
                            </ul>
                        </div>
                        <p class="letra px-5">
                            ¿Estás listo para entender cómo funciona el mercado
                            cripto? No operes con emociones. Aprende las
                            estrategias y disciplínate para ser rentable en este
                            mundo.
                        </p>
                    </div>
                </div>
            </div>
            <div class="col-sm my-auto">
                <div class="flex2 d-flex justify-content-center">
                    <img
                        src="img/47.png"
                        alt=""
                        class="img-fluid"
                        style="min-width:300px"
                    />
                </div>
            </div>
        </div>
    </div>
</section>

<div class="container-fluid bg-dark mt-3">
    <div class="container">
        <p class="pt-3 text-lg-center text-white letra2">
            ¿Deseas participar en nuestros talleres y señales gratuitas ? solo
            debes registrarte y obtendras acceso a la sala.
        </p>
        <div class=" mx-auto pb-5" style="max-width:1000px;">
            <button
                type="button"
                class="btn btn-primary"
                data-bs-toggle="modal"
                data-bs-target="#exampleModal"
            >
                <h5 class="letra">Registrate aquí.</h5>
            </button>
        </div>
    </div>
</div>

<!-- SERVICIOS -->

<div class="container-fluid bg-white">
    <span name="servicios" id="servicios" />
    <div class=" py-5  ">
        {#if coins.length > 0}
            <h2 class="ms-lg-5">
                <img
                    src={coins[0].image}
                    alt={coins[0].name}
                    style="width: 5rem;"
                />
                {coins[0].id.toUpperCase()}
                <strong> {coins[0].current_price.toLocaleString()}</strong> US$
            </h2>
        {:else}
            <p>Cargando...</p>
        {/if}
        <h2 class=" text-black text-center py-2 " style="font-size: 3rem;">
            <strong>Nuestros Servicios</strong>
        </h2>
        <p class="container py-1 letra2" style="">
            En cripto aprendes encontraras una variedad de soluciones, con
            nuestra experiencia te ayudaremos a ser rentable en este mundo de
            criptomonedas. Aprenderas nuestros métodos y pondrás en práctica
            estrategias que nos han funcionado durante nuestra trayectoria. No
            solo aprenderás trading, Tambien encontraras talleres sobre remesas
            y tips prácticos.
        </p>

        <div class="contenedor-cards1">
            <div class="news-cards">
                <div class="container">
                    <div class="row">
                        <div class="col-md">
                            <div
                                class="card  text-white mx-auto my-4 border-0  "
                            >
                                <a href="/trading" class="mx-auto"
                                    ><img
                                        src="img/19.png"
                                        class="rounded  card-img-top p-3"
                                        alt="..."
                                        style="max-width: 220px;"
                                    /></a
                                >

                                <h5
                                    class="card-title text-black text-center letra"
                                >
                                    <strong>Curso de Trading</strong>
                                </h5>
                                <div
                                    class="card-body bg-black rounded "
                                    style="min-width: auto;"
                                >
                                    <p
                                        class="card-text text-white letra"
                                        style="font-size: 1.5rem;"
                                    >
                                        ¡Invierte en tus conocimientos! Aprende
                                        todo lo que necesitas saber para operar
                                        en el mercado de las criptos con
                                        asesoría ilimitada.
                                    </p>
                                    <a
                                        href="trading"
                                        class="btn btn-primary letra "
                                        style="font-size: 1.5rem;">Leer más</a
                                    >
                                </div>
                            </div>
                        </div>

                        <div class="col-md">
                            <div
                                class="card mx-auto my-4 border-0 "
                                style="min-width: auto;"
                            >
                                <a href="/senales" class="mx-auto"
                                    ><img
                                        src="img/20.png"
                                        class=" rounded mx-auto card-img-top p-3"
                                        alt=" ..."
                                        style="max-width: 220px;"
                                    /></a
                                >

                                <h5
                                    class="card-title text-black text-center letra"
                                >
                                    <strong>Señales para Operar</strong>
                                </h5>
                                <div
                                    class=" card-body bg-black rounded"
                                    style="min-width: auto;"
                                >
                                    <p
                                        class="card-text text-white letra "
                                        style="font-size: 1.5rem;"
                                    >
                                        ¡No hagas trading solo! Membresía VIP
                                        por 30 días para obtener una
                                        recopilación de las mejores señales del
                                        mercado de criptomonedas.
                                    </p>
                                    <a
                                        href="/senales"
                                        class="btn btn-primary letra"
                                        style="font-size: 1.5rem;">Leer más</a
                                    >
                                </div>
                            </div>
                        </div>

                        <div class="col-md">
                            <div
                                class="card mx-auto my-4 border-0 "
                                style="min-width: auto;"
                            >
                                <a href="/senales" class="mx-auto"
                                    ><img
                                        src="img/21.png"
                                        class=" rounded mx-auto card-img-top p-3"
                                        alt=" ..."
                                        style="max-width: 220px;"
                                    /></a
                                >

                                <h5
                                    class="card-title text-black text-center letra"
                                >
                                    <strong>Remesas</strong>
                                </h5>
                                <div
                                    class=" card-body bg-black rounded"
                                    style="min-width: auto;"
                                >
                                    <p
                                        class="card-text text-white letra "
                                        style="font-size: 1.5rem;"
                                    >
                                        ¡Hazlo tú mismo! Aprende a enviar tu
                                        dinero desde cualquier país a otro,
                                        convirtiendo tu dinero en USDT de forma
                                        rápida y segura.
                                    </p>
                                    <a
                                        href="/senales"
                                        class="btn btn-primary letra"
                                        style="font-size: 1.5rem;">Leer más</a
                                    >
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
<Footer />
