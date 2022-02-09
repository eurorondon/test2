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

<div class="container-fluid bg-white">
    <div class="row">
        <div class="col-md-9">
            <div class="flex2 d-flex justify-content-center">
                <img src="img/boti.png" alt="" class="img-fluid" style="" />
            </div>
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Modi,
                repudiandae laborum sit quisquam, iste similique et ad,
                cupiditate unde dolores perferendis. Animi, assumenda? Corrupti
                quo molestias nulla ipsum sed a, cum amet temporibus impedit,
                delectus obcaecati molestiae officiis fugiat alias fuga, nihil
                culpa quae minima fugit rem. Perspiciatis tempora ipsam
                accusantium quaerat voluptate vero totam soluta in quam alias!
                Corrupti est, iste autem illum esse exercitationem voluptatem
                accusamus cum, quasi sapiente blanditiis rem excepturi! Ut
                nesciunt porro quod? Est animi pariatur molestias obcaecati aut
                molestiae perferendis reiciendis vero dolorum corrupti
                provident, ipsam iusto cumque, repellat magnam eligendi quasi,
                ad praesentium? Sed dicta, placeat deleniti molestiae ad magnam,
                voluptatibus cum amet dolorem omnis maxime numquam aliquid velit
                officiis quasi asperiores fugit? Ipsa dolores autem provident
                eius eligendi! Cum nisi quidem, error earum autem iste
                cupiditate sequi molestiae ipsam eaque sapiente debitis
                quibusdam aliquid tempora? Quam non illo corporis sint culpa
                officia rerum, aliquam laborum quis quo illum consectetur itaque
                eligendi sed tempora ipsum dolorem, sequi commodi suscipit?
                Fugit provident quasi, omnis rerum vel veniam magnam similique
                aut dicta nesciunt voluptates eum asperiores distinctio dolore,
                dolor sequi culpa, aliquid quo impedit nulla. Illo enim
                exercitationem quidem laudantium quo. Recusandae facilis error
                pariatur voluptates consequatur, ipsum dicta, cum soluta, alias
                nesciunt modi similique commodi libero neque facere. Earum
                aliquam quo tempore, illum quasi distinctio fugit eveniet
                itaque. Praesentium omnis aut sint, assumenda delectus tempora
                nihil eius. Recusandae facere corporis voluptate, perferendis ea
                quas, porro, optio tenetur quaerat ipsam voluptates quo debitis
                corrupti sapiente delectus voluptatibus reprehenderit commodi
                error cupiditate inventore? Optio provident error iste
                exercitationem deserunt architecto facere sunt adipisci earum
                dolores nisi, eveniet necessitatibus, quo doloremque et magnam
                quibusdam facilis consequatur maiores! Doloremque, explicabo
                placeat laboriosam blanditiis commodi reiciendis illo dolor quod
                veniam incidunt. Dicta quibusdam eveniet dolore obcaecati
                doloribus at quas debitis enim necessitatibus laborum, esse
                tempora quidem minus distinctio alias voluptatibus a maiores
                libero soluta ipsa corporis fuga perferendis incidunt! Nostrum,
                unde ratione similique natus impedit totam sapiente amet
                suscipit neque accusantium sit corrupti esse autem? Deleniti
                commodi velit architecto nobis veritatis consectetur, eaque
                ullam ab odit provident facilis vero magnam ad rem at sed nihil
                dolorem voluptate excepturi quo expedita aspernatur doloremque?
                Necessitatibus explicabo quae soluta fuga libero saepe magni
                aliquid quibusdam adipisci nostrum voluptatem cum sapiente velit
                at alias repellendus ea officia nulla cumque, rem labore?
                Accusantium numquam fugit, quibusdam sunt amet perspiciatis,
                minima totam reiciendis consequatur sit itaque molestias
                quaerat! Error accusantium corporis quos vero laborum quisquam
                voluptate nobis minima nisi cum sint sapiente labore repellendus
                voluptas, a quas iure? Quasi alias sit ipsum vitae sint non
                veniam ducimus, ratione eius accusantium atque nisi possimus eos
                dicta maxime ex cum repudiandae exercitationem voluptas totam
                quibusdam provident est quod optio. Debitis placeat cum libero
                expedita excepturi, non ad eveniet fugiat eum quisquam nam
                sapiente labore commodi a error autem doloribus cupiditate
                consequatur? Vel recusandae quae qui non, unde dolorem maxime
                enim sed, praesentium voluptas perferendis! Iure doloribus
                asperiores expedita et commodi veritatis ratione quam incidunt,
                molestiae iste minima facere hic at sint placeat magni aliquam
                ullam perferendis voluptatibus. Dicta perferendis alias eaque
                error nesciunt, facere in ex officiis laudantium mollitia eum
                quidem reprehenderit laborum quo a nisi? Cupiditate facere vitae
                dolorem incidunt nemo dolores, quidem, qui beatae, dicta cum eum
                perspiciatis natus a! Veritatis voluptatum dolorem, eum pariatur
                ducimus at tempore dolor repellat praesentium, nam nisi
                explicabo eius totam sequi eveniet cum porro consectetur, minus
                suscipit. Autem, quo. Autem error impedit eaque similique nobis
                harum distinctio natus suscipit sit, aperiam, aspernatur
                reprehenderit! Dolor, cum ipsa cumque eos nobis quis
                necessitatibus perferendis non distinctio eius quod, esse
                deleniti ut id! Placeat odit explicabo doloribus suscipit
                voluptatum omnis consequatur esse nam deserunt repellendus
                perferendis dolore maiores assumenda voluptatibus, saepe itaque
                earum dignissimos autem, tempore fuga quibusdam. Quis, labore
                quaerat aliquid ullam sunt doloremque quo incidunt eum fuga
                voluptatem porro reprehenderit blanditiis? Eum distinctio iure
                culpa blanditiis quaerat ratione. Qui, error! Dolore a nam
                assumenda illo possimus molestias autem quo ratione accusamus
                eaque tempore molestiae quasi ab animi facilis voluptatem
                nostrum, sapiente eum. Repudiandae sequi tempore maxime facere
                repellendus sit repellat dolor asperiores cupiditate commodi
                modi eius consequuntur omnis, aperiam quidem aliquid ad fugiat
                facilis saepe dignissimos expedita architecto accusamus
                laboriosam! Consequuntur magni qui minima laboriosam maiores rem
                iste voluptas ipsum distinctio libero, eius aliquid tempore
                accusantium! Quae debitis laudantium velit, maxime dolorem non
                mollitia alias fugiat, temporibus autem impedit dolores? Vel
                unde quisquam sequi! Aperiam maiores, debitis delectus nostrum
                explicabo exercitationem voluptatum suscipit ea hic rerum
                tempore, molestias eligendi commodi ab corrupti maxime quaerat
                voluptatibus vitae molestiae deserunt! Numquam voluptates
                consequatur aliquam officia dolor ipsa saepe, deserunt expedita
                atque vel quaerat libero non quibusdam debitis ex eos odio sit
                voluptas accusamus porro eveniet beatae corrupti. Magnam
                laudantium sint, facere atque inventore dolores beatae culpa
                quos cupiditate, placeat enim accusantium quas soluta! Velit,
                delectus ea ducimus repellendus asperiores nesciunt illo sit
                totam recusandae similique veritatis vitae id dolorem sapiente
                doloremque ab nostrum quibusdam maxime temporibus. Consectetur
                recusandae debitis facilis nihil alias animi! Ut nam similique
                magnam vitae explicabo voluptas distinctio assumenda corrupti
                doloribus perferendis, doloremque, deleniti molestiae
                exercitationem velit enim modi numquam autem aliquam. Ipsam sint
                aliquid vero nobis illo, deserunt sunt cupiditate, molestias
                laudantium nulla amet libero? Eligendi totam saepe ab adipisci
                modi, blanditiis odio labore necessitatibus. Eaque incidunt
                inventore officiis distinctio, odit numquam fugiat! At molestias
                nobis earum nemo repellat, quo libero ea minus nihil? Quaerat
                totam est expedita sequi suscipit molestias ipsa iure!
                Consequuntur repellat corporis voluptates esse explicabo a
                cupiditate inventore nihil incidunt voluptatibus eum voluptatum
                temporibus deserunt consequatur, error dolore eaque harum rem
                et. Inventore modi eveniet labore aut dolores consectetur, ad
                tenetur minus odio distinctio, alias reprehenderit deserunt vel
                voluptates perspiciatis, deleniti sapiente iusto ipsam.
                Necessitatibus repudiandae neque asperiores! Molestiae modi a
                magnam soluta nam et veritatis id illum nisi dolorum, eum animi
                dolor. In rerum molestias adipisci atque natus earum, harum
                obcaecati dolorum. Doloremque quae in, deleniti, vero repellat
                deserunt laudantium corporis officiis modi soluta commodi
                assumenda voluptatem, dicta reprehenderit praesentium iure sit!
                Id ullam dolore quidem laboriosam, non autem iure rem et eius,
                necessitatibus repudiandae ipsa. Ea recusandae tempore labore
                repellendus tenetur quos iure molestiae perferendis quibusdam,
                iste ab sapiente, fuga minima nobis nemo dicta quaerat veniam ex
                nihil. Reprehenderit natus temporibus quas commodi odio dolorum,
                minus deleniti possimus fugiat debitis doloribus sit omnis est
                at accusamus voluptas suscipit magni voluptates nobis tenetur
                culpa adipisci. Quos corrupti ratione nesciunt quam odit quaerat
                sequi libero dicta possimus sunt ad excepturi velit corporis nam
                officiis et adipisci esse veritatis eum, vel officia provident
                quo impedit! Quasi rem enim pariatur aspernatur, nostrum in, a
                numquam sit quis cumque hic nam recusandae eum suscipit! Quo
                officiis fugit eius provident animi velit sit id autem officia
                nobis soluta dolorum debitis natus iste, laudantium suscipit
                unde aut, accusamus quasi. Illo eveniet, rerum amet architecto
                necessitatibus animi sit nemo reprehenderit corporis dolorum at
                rem deserunt ratione tempore aut quos tempora atque numquam
                dolor? Molestias dolor alias impedit. Illum aspernatur
                voluptatibus nihil aut sequi est amet vero ducimus animi, eius,
                ab placeat enim hic praesentium maiores nemo quas, provident
                sint! Expedita inventore harum quis reiciendis quod labore
                perspiciatis tempore optio aspernatur asperiores id impedit
                recusandae voluptas fugit nam, fugiat, beatae voluptatem
                cupiditate, aliquam non consequatur culpa adipisci. At, deserunt
                in pariatur quisquam, tempore commodi sequi recusandae soluta
                ullam unde autem incidunt? Enim, temporibus molestiae sunt
                libero laboriosam fuga quis. Aut numquam sed, facere
                reprehenderit quasi delectus molestias dolorum quo nulla veniam
                provident. Odit quia ipsa nam unde dolorum repudiandae cumque
                itaque officiis sapiente? Dolore in dolorum et doloremque harum
                iste corporis architecto sunt molestias. Recusandae sint dicta
                incidunt quis deserunt quisquam nobis hic beatae doloremque.
                Tempore tenetur nesciunt porro corrupti molestiae nulla,
                voluptatem, eveniet aspernatur provident quam velit nemo nostrum
                placeat sed, inventore atque aliquam a autem molestias vero
                alias qui doloremque rem? Corrupti laudantium distinctio culpa
                iste magnam quisquam aliquid suscipit molestias commodi, nihil
                quia consequatur eum pariatur? Maxime vero quas nostrum eveniet
                recusandae cum ducimus saepe ullam numquam nihil, excepturi
                adipisci ea soluta harum ipsa, ipsam voluptas quos enim!
                Delectus debitis hic quo. Iusto doloribus doloremque aperiam
                temporibus dolor perspiciatis veniam magni sint error dolorum?
                Id, officia sapiente. Mollitia hic fugiat cumque modi ut dicta
                at necessitatibus sapiente possimus consequuntur, inventore rem.
                Ab ducimus quis eligendi quo. Adipisci, aliquid autem ex ullam
                magnam repellat sit vitae eum assumenda, illo laboriosam ipsum.
                Officiis ullam pariatur voluptate porro ipsum quasi voluptas
                autem minus quisquam in debitis reiciendis optio vero soluta
                perspiciatis recusandae delectus error praesentium, nam eius
                distinctio dicta natus molestias laboriosam! Expedita, saepe
                accusamus deserunt quam dignissimos minus consectetur a ipsam
                deleniti nobis assumenda necessitatibus ab, unde, fugiat sint?
                Minus magni dignissimos saepe odit ex rem. Placeat quasi, ipsum
                harum aliquid, adipisci recusandae enim ullam earum commodi
                sequi vitae hic. Debitis consequatur maiores dolores aperiam
                quis. Eveniet rerum itaque cum dicta earum repellat iusto quae
                cumque aliquid maiores alias nostrum eaque eum numquam, corporis
                quasi nesciunt excepturi quisquam perspiciatis, nulla magnam
                harum quia. Nisi, dolore quae et itaque sed voluptatem cum ad
                nostrum quod delectus sit asperiores laudantium ut tempore iusto
                at dolorem voluptate, reiciendis ipsa placeat similique
                aspernatur ipsum repellendus minus. A assumenda doloribus earum,
                aspernatur ducimus exercitationem pariatur sint itaque. Vel
                soluta doloribus sapiente officia quasi doloremque fuga
                molestias blanditiis ipsa veniam. Eligendi repellat natus sit
                quas quae voluptatibus quam debitis autem, consequatur
                distinctio, in, error sequi fuga commodi. Explicabo, ratione?
                Quis ut sit illo, explicabo, iste deserunt dolor voluptatem
                dolorem suscipit, dolorum non voluptate odio nisi hic officiis
                aut consequuntur qui. Sint eveniet sunt aperiam, quos
                repellendus quae odit maiores nemo harum corrupti, ducimus eius
                fugit necessitatibus debitis ad qui possimus excepturi doloribus
                temporibus voluptates facere est quia sapiente fugiat. A at
                eveniet quae ab dolorum repellat facere ullam, maiores totam!
                Quaerat rem asperiores illum odio deserunt quod voluptatem
                perspiciatis quibusdam ullam, aliquid, sapiente dolore, eius
                corporis explicabo aut praesentium officia nisi ad accusamus
                laborum pariatur natus vero cum at. Voluptatibus illum maiores
                dolorum asperiores minima. Recusandae possimus provident sint
                incidunt libero ratione. Ut ratione quo, odit corporis nemo
                omnis qui sapiente libero, mollitia temporibus ducimus non
                facere quos suscipit ab quidem molestiae error, numquam
                quibusdam. Laboriosam, culpa autem est ea labore pariatur
                consectetur tenetur dolor sed dignissimos dolore laudantium
                praesentium totam aspernatur voluptatem doloremque eum corporis
                omnis modi ipsum. Est optio corporis nobis ipsam, aliquam
                quaerat totam vero, temporibus omnis veritatis voluptate
                adipisci sunt voluptatem, saepe iste? Laudantium, aspernatur
                distinctio odio accusamus numquam dolorem consectetur minus
                nulla magni odit unde, tempora neque! Consequuntur, vitae!
                Explicabo numquam aut eum dolor nisi incidunt accusantium ipsum
                quis iste, alias eaque, quaerat reiciendis blanditiis, minus
                aliquid adipisci repellendus quae quod velit nihil enim illum
                aperiam. Expedita labore minus hic ipsam soluta quas incidunt
                quaerat laborum animi, eum cumque, ipsum commodi molestiae atque
                iusto, temporibus voluptates nam? Iure doloribus ad provident
                itaque. Facilis ex quis minus porro recusandae quo libero. Aut
                eligendi vel magnam velit ab quasi, nostrum ad! Sit, eum iure
                maxime ab perferendis eius blanditiis id fugiat accusamus
                nostrum minima, cumque rerum exercitationem vel, ipsum mollitia
                sed modi possimus neque quisquam nisi dicta accusantium veniam
                reprehenderit. Doloribus pariatur provident culpa expedita
                exercitationem temporibus, saepe praesentium quasi et laborum
                dolores tempora beatae, adipisci esse maxime laudantium a nisi
                fuga aut? Saepe animi, neque molestiae unde sit repellendus,
                culpa dolorem maxime amet optio beatae. Provident voluptatibus
                laboriosam sint laborum aspernatur! Sed debitis molestiae alias
                temporibus natus quisquam est fugit suscipit dolores incidunt,
                aliquam nulla repellat earum, odit nihil ad error sunt quaerat.
                Eveniet aspernatur molestiae tempore quo. Aliquam unde qui ab
                accusantium quas porro natus earum? Eveniet molestiae
                consequatur sed id reiciendis nesciunt distinctio, sapiente
                maiores amet eos iure, quo impedit aliquid dicta similique nihil
                odio obcaecati! Magnam pariatur aliquid dolores, voluptas
                repudiandae vel suscipit, perferendis assumenda ratione ea
                explicabo, voluptatum ex odio minus dolorum soluta modi?
                Perferendis veniam rem distinctio amet explicabo itaque commodi
                officia doloribus inventore? Voluptates, accusantium atque
                tempore vel voluptatibus nemo id mollitia hic dicta! Fugit, a
                nulla exercitationem nostrum ipsum tempora magni ducimus fugiat
                natus ex, facere veritatis officiis, modi rem ut deserunt
                blanditiis suscipit ad. Quisquam, eos. Voluptatem culpa incidunt
                sapiente nisi totam asperiores sint voluptatum magnam, quae
                necessitatibus aperiam esse laborum minus quasi vel dolorum cum
                deserunt ea nostrum iste tenetur perferendis! Soluta autem, nam
                possimus magnam quibusdam laboriosam iste. Dicta consequuntur,
                quasi, mollitia dolorem hic molestiae dignissimos nesciunt
                atque, quidem dolorum cupiditate odio. Sint accusantium nulla
                delectus vel provident adipisci maiores ducimus laboriosam fugit
                deserunt molestias harum et amet quis commodi repellat nesciunt
                pariatur, tenetur fuga consectetur esse quas voluptatibus ipsam
                ea? Ratione quia eos neque iusto ut nesciunt expedita modi earum
                temporibus, eius magni ipsam reprehenderit doloribus placeat
                quam ducimus, optio fugit aperiam! Sit quisquam reiciendis
                facilis debitis ipsam. Commodi similique labore sunt vel sint
                magnam dolore delectus distinctio dolorem, suscipit sapiente
                esse illum possimus amet consequatur obcaecati veritatis dolorum
                debitis magni aspernatur iure? Repellendus, corrupti! Velit
                accusantium nam laborum sit blanditiis dolores quidem doloribus,
                ullam inventore quae fugiat, recusandae consequatur porro. Ipsa
                adipisci voluptatem esse veniam quibusdam autem hic tempora sit
                explicabo modi doloremque aperiam obcaecati facilis maxime, odit
                dolor. Minima dignissimos labore vero nihil nostrum, magnam fuga
                culpa aspernatur doloremque amet incidunt rerum autem sunt
                facilis debitis! Nulla quam iure laborum, similique labore
                ratione sequi. Explicabo eveniet quas autem error rerum delectus
                provident saepe quidem ad fugit neque accusamus sequi et
                quibusdam expedita nisi, odit earum ducimus reiciendis
                dignissimos, possimus perspiciatis iure doloribus distinctio?
                Repellendus accusamus vel quas quo non laborum dicta voluptatum
                iure repellat quis numquam aliquid fugiat esse sit
                necessitatibus officia quod nam voluptatem deserunt, nisi
                dolorem ea labore ut debitis? Quibusdam maxime reiciendis
                accusantium provident at possimus, praesentium veniam laudantium
                est animi architecto recusandae ab consectetur ex cum fugit
                voluptate minus hic et? Non hic porro, deserunt fuga consectetur
                modi esse harum voluptatibus impedit in cupiditate mollitia
                libero corrupti dolore. Adipisci eius ex, sed officiis similique
                excepturi consequatur deserunt explicabo impedit eaque aperiam
                ea debitis quasi illum culpa sequi magnam amet distinctio
                voluptate nihil enim. Libero tenetur quae necessitatibus omnis
                explicabo dolor eius cum sit, suscipit earum qui at laudantium
                natus eligendi odit. Libero at, recusandae nostrum quia sint
                laudantium fugit officiis repellat beatae suscipit unde
                veritatis non facere aut ea placeat vel, ab inventore et
                dignissimos, qui culpa. Minus vel excepturi veritatis itaque
                minima et quam nobis deserunt odio animi odit molestiae mollitia
                temporibus incidunt architecto ea optio doloribus, dolor iusto
                hic beatae necessitatibus earum suscipit. Accusantium fugit et
                molestiae aut consectetur labore beatae. Sunt amet enim hic
                aliquam, at voluptatem aspernatur laudantium ex nisi velit sequi
                provident sit maxime ipsum ut assumenda deleniti, accusantium
                soluta iure commodi? Tempore suscipit nemo cupiditate
                exercitationem nihil neque dignissimos nisi. Natus, possimus at
                consectetur reprehenderit illo, hic voluptate optio distinctio,
                minus commodi aut nisi qui excepturi labore voluptas quos
                architecto explicabo ipsum! Repellat magnam quisquam quas iusto
                cum possimus sequi odio commodi soluta! Corrupti in ea amet non
                officia accusamus modi, a officiis ullam nihil, inventore sit
                minus aliquam, quibusdam ab nesciunt illum qui ipsum harum.
                Ullam commodi eligendi repudiandae voluptate ad sapiente totam
                nihil dicta nemo, magnam cupiditate perspiciatis autem quis
                dolore quam. Nulla, officiis! Commodi, explicabo cumque
                dignissimos sit repudiandae officiis nesciunt voluptates. Nihil
                laborum dignissimos at! Corporis, inventore quibusdam earum cum
                eligendi molestiae laboriosam, expedita dicta sapiente magni
                eius libero deleniti. Minima pariatur esse animi praesentium
                repudiandae iure sequi quisquam. Veritatis sapiente labore illo
                incidunt debitis est harum eaque iure pariatur ab. Fugiat quod
                animi, odit esse, provident rem nemo cumque, tempore consectetur
                soluta accusamus quaerat ipsa pariatur eaque iste quia aliquam
                voluptate minus laudantium. Nam ipsum laborum voluptatibus porro
                veritatis. Excepturi dignissimos molestiae quod autem. At ullam
                nulla est totam beatae, et sed obcaecati fugiat doloremque
                aliquam earum unde perspiciatis, placeat ipsam. Totam quibusdam
                doloribus, vitae sit facilis eaque, tempora esse ullam inventore
                modi quia? Adipisci recusandae voluptatem labore velit fugit
                itaque ex natus, repellendus quia error provident facilis
                molestias, incidunt quas sed doloribus. Excepturi cupiditate,
                rem deleniti ea, similique impedit sapiente, reprehenderit ut
                soluta adipisci nesciunt quod. Quis accusantium facilis ipsam,
                perferendis nam possimus iure omnis, vero a ratione fuga.
                Repudiandae laboriosam totam iure modi, sapiente nobis, at
                voluptatem, rem libero quasi praesentium. Harum nisi unde
                excepturi accusantium deserunt odit, modi sequi, quibusdam vero
                debitis sunt doloremque quae tenetur laboriosam iure
                perspiciatis accusamus quaerat. Aspernatur voluptatibus nobis
                quae error dignissimos distinctio, earum vel veritatis quisquam,
                ex iusto eius inventore, optio vitae deleniti possimus. Est
                doloribus mollitia ipsum ut quos, dolor delectus eaque
                reprehenderit eum tenetur rerum illo aspernatur blanditiis
                laboriosam facilis corporis tempora doloremque adipisci?
                Repellat quam rerum consequuntur voluptate commodi! Nobis
                tempore animi commodi corrupti blanditiis error quidem similique
                reiciendis quibusdam nesciunt? Quaerat dolores consequuntur enim
                provident dolorum doloremque, hic exercitationem quis ut
                repellendus at corporis. Qui illo iste ea minus voluptatum
                voluptatibus officiis accusantium, aperiam, quas nam
                praesentium! Labore molestiae praesentium eius amet. Molestiae
                nulla qui deleniti ab enim illum. Recusandae, dicta accusamus
                porro consequuntur consectetur officiis vero repudiandae iure
                voluptatibus velit sit culpa eius ducimus numquam, debitis
                maxime voluptatem odit sunt quibusdam. Enim, aliquid velit.
                Autem, enim itaque eius distinctio nihil sed saepe similique?
                Ipsam corrupti nobis molestiae architecto deleniti cupiditate
                mollitia? Veritatis quibusdam iste dolore ab, autem provident
                voluptatibus quam sequi. Laborum, praesentium reiciendis.
                Impedit aut quo maxime eos laudantium dolorum dolore ab
                eligendi. Quibusdam molestiae officiis praesentium distinctio
                ipsa minima nostrum laborum, ad eligendi, reiciendis maiores
                ratione quisquam quia labore impedit fugit dolores placeat
                voluptas enim mollitia repellendus? Modi distinctio error
                eligendi quas necessitatibus corrupti animi beatae cumque quasi
                similique sed, earum quo in nobis sequi possimus, reiciendis
                quos asperiores autem vel libero sunt optio fugit tempora.
                Aliquam, minus soluta omnis sequi officiis animi sit nobis
                temporibus atque reprehenderit blanditiis quaerat nesciunt odio
                tenetur vero quibusdam aspernatur consectetur ratione saepe ea
                ducimus enim dolore expedita? Vero, voluptate nesciunt
                accusantium nemo iure similique dolorum aliquid autem voluptates
                enim quia natus architecto non necessitatibus repellendus
                aliquam et eum minima sit dicta optio reprehenderit blanditiis
                atque exercitationem! Earum molestias praesentium tempore,
                voluptatum laudantium rem ipsum. Ratione, ipsa nisi, expedita
                veritatis quo quam nam et fugit quis nemo optio nulla quaerat
                possimus molestias architecto eius nihil quod nesciunt commodi
                ullam repellat minus voluptates obcaecati mollitia. Voluptatum
                adipisci tenetur mollitia unde fugit quo dicta quasi. Dolor
                explicabo ad officia, fugit aut, eveniet, nam doloremque alias
                at amet facilis rem repellat ab pariatur blanditiis! Dolor
                maxime molestias dicta at sunt, rem quasi, excepturi beatae
                nostrum illo est nam quisquam rerum, error quod odit voluptates?
                At quidem unde dolor animi mollitia fugit eum doloremque quod.
                Enim sequi aliquid nostrum dolorum voluptates dolorem harum
                voluptate velit? Voluptate facere cum dolores blanditiis dolorem
                placeat totam. Magnam iste sapiente et! Voluptate corrupti amet
                quo! Quae repellat illum sed amet porro laborum excepturi, iste
                facilis, corrupti aliquam veniam repudiandae? Consequuntur
                deleniti ab omnis facilis quasi at consectetur, adipisci ducimus
                architecto et rem consequatur suscipit eius possimus accusamus
                veritatis dolore sit odit aliquid tempora laborum. Numquam
                harum, facere sapiente adipisci quo consequuntur qui quaerat
                maxime sit rerum expedita architecto vero et nemo repellendus
                praesentium modi, error quibusdam eius incidunt, voluptatibus
                voluptas sunt voluptates? Voluptates delectus cum ratione atque
                voluptatum asperiores fuga distinctio quaerat corporis
                laboriosam, alias tempora facere aliquid laborum ea deleniti
                eius labore earum illum itaque sapiente esse cumque. Dolores
                repudiandae perferendis doloribus laborum perspiciatis, maiores
                recusandae ab, commodi eius velit tempore sunt architecto odio
                rerum esse. Est quibusdam architecto assumenda in libero
                doloremque deserunt voluptatum eum officia expedita
                exercitationem, a unde vero itaque. Consequatur vel molestiae
                corporis itaque, consectetur maxime tempore delectus ad sed
                explicabo praesentium non ut aspernatur alias animi ratione
                dolorum at eum! Perspiciatis, optio, natus sint iusto tempore
                facilis a nesciunt cumque sit vero consequuntur cupiditate,
                mollitia voluptas illo. Nostrum voluptatibus nulla libero, sint
                illum incidunt modi quidem officia dicta atque aperiam neque
                unde accusantium impedit beatae doloremque voluptatum, possimus
                explicabo tempore nobis soluta aliquid deleniti. Aliquid numquam
                laborum sed asperiores eos iste qui, earum voluptatum esse? In,
                ab! Possimus assumenda, asperiores officia voluptate ipsum
                minima amet, qui quaerat voluptatum iste modi reprehenderit
                doloribus? Neque fugit dicta temporibus natus eligendi
                praesentium voluptas aliquam tempora dolore repudiandae ipsum
                perspiciatis eos est dolorem, fugiat cupiditate! Iure maiores,
                facilis autem vel nostrum possimus inventore enim eos
                accusantium consequatur repellendus, temporibus unde architecto
                nemo eaque incidunt voluptatem atque nulla distinctio laborum
                optio sequi deserunt fugiat. Nisi modi enim fuga nemo
                consequuntur tempora sequi, odio commodi nam dicta labore
                quisquam distinctio ex, rerum, ducimus deleniti architecto
                delectus quas velit. Debitis iure aut rerum id incidunt tempora
                praesentium sed eaque, optio laborum magnam illum libero beatae
                numquam voluptatum? Nisi culpa corrupti harum alias quam iure
                vero excepturi distinctio, aliquam labore optio laudantium quos
                temporibus repellat commodi. Laudantium accusantium nisi
                molestias in fugit, quo nobis esse veniam fuga obcaecati unde et
                maiores iste ex eius voluptatibus cupiditate dignissimos nam
                adipisci aliquam, magnam eaque porro. Ad, commodi nesciunt
                voluptatem vero blanditiis quis labore repudiandae culpa, rem,
                dolores fugit quae reiciendis quaerat facilis ut aliquam
                similique facere eum quia exercitationem voluptatibus corrupti
                fugiat! Explicabo facilis quidem autem soluta voluptatibus neque
                reiciendis laudantium. Quas nam delectus ipsum possimus!
                Deserunt libero voluptatum perspiciatis eius natus delectus
                corporis quis inventore, adipisci maxime sapiente,
                exercitationem, voluptate alias soluta voluptas mollitia
                accusantium nam cumque officia cum asperiores quaerat!
                Voluptatum amet culpa beatae earum iure odio provident enim
                sapiente laudantium officiis pariatur voluptate inventore
                quibusdam perferendis aliquid aspernatur reprehenderit quam
                eaque consequatur incidunt, cupiditate expedita. Voluptatem
                tempora ad ullam fugit exercitationem illum veritatis ex
                quisquam incidunt ab harum quibusdam eius molestias culpa, nam
                non? Quas neque voluptatum, corrupti eos pariatur enim porro
                tempore consectetur, eum nobis molestiae quaerat ad earum nulla
                sint, corporis molestias rem? Tenetur, quod obcaecati iure
                magnam doloribus facilis corrupti atque veritatis eveniet ad
                eaque voluptatum earum dicta eum ducimus debitis laudantium
                ullam nam eius aut modi? Totam excepturi tempora consequatur
                modi eum reiciendis harum consectetur inventore blanditiis nihil
                velit vitae doloremque quam repellendus quis illo, quod veniam
                asperiores, officiis perspiciatis ipsa! In tenetur accusantium
                deleniti quaerat eos odio. Ad unde excepturi iusto quas
                reprehenderit corporis neque, reiciendis ab corrupti quidem
                eligendi hic, rerum quia amet magnam numquam aspernatur?
                Temporibus soluta fugit laboriosam odit, facere odio ullam
                adipisci ut praesentium ad doloremque nulla quae! Placeat eum
                totam qui, cupiditate error quasi excepturi iure, dolorum nemo
                aspernatur fugiat nihil eos voluptatum accusantium in at! Fuga
                nemo eius illum rem sit veniam obcaecati saepe, quam velit ipsam
                aut vel consequatur architecto at nesciunt, praesentium quia
                dignissimos facilis repellat porro facere! Nam aspernatur quasi
                earum nostrum temporibus, dolorum ipsam illum rerum sapiente
                nesciunt expedita repellendus veritatis, eligendi officia alias.
                Nulla corporis quisquam ipsa. Fugiat alias maiores veniam,
                nostrum pariatur facere cupiditate unde assumenda sint ab,
                voluptatum voluptates, impedit aperiam vel modi quam quo
                sapiente ipsa corrupti! Nulla, aperiam quas! Tenetur temporibus
                ipsum soluta eius quo nulla. Impedit inventore maxime cumque
                nobis fuga quis officiis alias eius eos quisquam blanditiis sunt
                quibusdam voluptate velit suscipit libero ut corrupti dicta,
                explicabo, architecto aliquid. Voluptate, nam quis itaque ea
                facilis assumenda ad inventore molestiae quae praesentium
                repudiandae veniam eveniet reiciendis dolor fugiat dicta!
                Placeat, ipsam omnis. Dolor veritatis temporibus soluta?
                Recusandae provident consectetur in error modi dolores
                consequuntur voluptate, nisi laborum, ipsam adipisci, eaque
                numquam quaerat illum ratione temporibus quasi odit est hic
                voluptatibus optio aut ipsum. Qui adipisci voluptas quod porro
                nemo perspiciatis eos labore fugit incidunt quis rem, pariatur
                ratione officiis deserunt nostrum nihil corrupti veniam nobis
                asperiores laboriosam illum, cum illo et. Architecto totam
                laboriosam possimus quae deserunt maiores numquam debitis labore
                cupiditate suscipit sint a, dicta voluptatibus. Accusantium,
                temporibus accusamus deserunt dolorum dignissimos voluptates!
                Enim ab rem quod expedita natus, vitae aperiam optio amet
                obcaecati unde sapiente deserunt nulla ad dolor a nam doloribus
                officiis accusantium ullam! Beatae quia expedita voluptate rem
                vero a libero nisi ad maxime? Odio cupiditate nulla saepe optio
                laborum cum dicta? Dolores quaerat sit provident autem ex?
                Tempora dolores iusto ratione provident, quia voluptates animi
                laboriosam recusandae id voluptas numquam dicta ipsa ea
                voluptatem iure, exercitationem sint sed necessitatibus? Alias
                consequatur temporibus placeat amet fugiat ab blanditiis modi
                facere expedita eum rerum eos vitae recusandae ut, dolorem,
                ipsum, exercitationem iure culpa omnis eius! Doloribus iste
                rerum aperiam ab cumque quisquam perferendis corrupti esse
                eveniet voluptates nobis suscipit repudiandae dignissimos veniam
                quasi asperiores expedita omnis placeat, qui laboriosam et nemo
                magni ad consequatur. Velit, minus incidunt? Corrupti fugit
                quidem quas magnam porro dolore tempore aperiam impedit vitae,
                enim reprehenderit tempora deserunt itaque nobis voluptates
                excepturi, odit assumenda quo magni modi soluta, similique
                beatae. Eius cum dolorum soluta officia alias id at dolor,
                tempore ipsa deleniti sunt? Ratione quaerat sapiente consequatur
                tenetur distinctio quis tempore porro deserunt! Placeat,
                perspiciatis magni. Sequi ratione, voluptatum veniam inventore
                repudiandae harum laudantium nobis. Hic sunt quibusdam nulla
                corrupti, consequuntur doloribus repellat adipisci fuga
                veritatis tenetur labore aspernatur repellendus id voluptatum.
                Commodi laborum deleniti illo ratione dolorum aspernatur
                perferendis, laboriosam explicabo harum ipsum quod. Iusto quidem
                error autem porro est voluptate, exercitationem aspernatur
                maxime repellendus nesciunt, nemo placeat suscipit cum assumenda
                culpa labore sint voluptates enim. Reiciendis sapiente libero
                accusantium, laudantium itaque quisquam laborum omnis ut quam
                tempore eius, ullam animi error commodi labore? Ea tenetur
                perferendis animi sunt est unde porro amet aspernatur, libero in
                eveniet molestias? Impedit sint ratione modi necessitatibus fuga
                vero molestias eos, commodi facere velit numquam, in debitis
                ipsa nesciunt quas id delectus optio voluptate sequi est ea
                eius. Modi soluta consequuntur blanditiis natus, fugit ipsam a
                dolores velit, fuga officiis aut maiores reprehenderit quis
                explicabo. Sapiente, cumque? At dolore odio iusto saepe magni
                quo delectus eius nostrum vitae nesciunt explicabo, quam minima
                eveniet consectetur magnam ad quaerat dignissimos id optio error
                cumque aut? Voluptates nisi autem animi delectus, sed incidunt
                perspiciatis. Excepturi doloribus harum sint animi temporibus,
                cum ea dolorem iusto earum quisquam ut quidem beatae placeat
                aperiam corrupti. Quos, ipsam eaque? Beatae, consequuntur
                cupiditate nesciunt, soluta unde id similique, eum est ratione
                velit hic cum. Consequuntur a eius, dicta modi ratione tempora
                obcaecati maxime, molestias harum odit, enim illo ducimus
                laborum assumenda alias vel eligendi. Consequatur impedit
                doloribus nam, in eaque aspernatur iure? Numquam eum tempora
                porro doloremque illum modi. Commodi iure quidem alias, veniam
                recusandae error magni? Ad dolorem quisquam illum dicta
                consequuntur optio neque eaque doloremque dolorum reiciendis
                porro quo, quae architecto corrupti nam fugiat rerum in
                consequatur molestiae vel nisi reprehenderit omnis hic.
                Officiis, odio eveniet voluptatibus eos quisquam et accusamus
                consequuntur id eius earum sint tenetur voluptatem. Sint soluta
                provident, harum rem iste minus odio possimus perspiciatis
                beatae consectetur tenetur veritatis accusamus. Corrupti
                repellendus fugiat velit atque voluptate, recusandae autem esse
                odio doloremque modi, saepe nobis aliquid reprehenderit?
                Accusantium quos commodi rerum similique fuga voluptatum laborum
                quisquam, ipsa sed aperiam architecto id dicta ex deleniti!
                Ullam expedita minima aliquam quos deserunt accusamus harum,
                itaque ab pariatur, ducimus voluptas reprehenderit velit atque
                inventore aperiam in! Odit obcaecati accusamus suscipit veniam
                magnam cum? Quas sed sint et veniam, neque consequuntur quisquam
                vero minus obcaecati ipsam, cupiditate tempora, odit blanditiis.
                Perspiciatis iste aliquam soluta obcaecati necessitatibus,
                pariatur porro nobis vero et. Blanditiis pariatur reprehenderit,
                quaerat totam odio atque id unde consequatur nihil repudiandae
                sit quod asperiores. Consectetur recusandae beatae magnam
                consequatur. Nesciunt rerum nam, facilis voluptas, consequatur,
                corporis error voluptates dolores pariatur in voluptate
                asperiores magni. Reiciendis consequatur, inventore facere ipsum
                repudiandae facilis esse iusto accusantium quae aliquam, dolore
                enim debitis et unde in quos ea praesentium asperiores sunt
                ducimus blanditiis! Veniam saepe aliquid voluptatem eos tempore
                accusantium, vero consectetur itaque a dolorem ab nulla quos
                iure ipsam nesciunt eius nihil. Repudiandae voluptates et autem
                praesentium? Libero corrupti ipsum veniam qui! Error tenetur
                mollitia perspiciatis, ab aspernatur, illum animi excepturi
                ipsum dicta, a suscipit. Officiis fuga voluptates pariatur quis
                perspiciatis possimus nisi delectus illum, corporis itaque
                assumenda, porro quam doloribus sapiente est inventore in
                deserunt impedit! Ut, non? Molestias neque iusto vero quos eum,
                omnis qui unde earum quaerat consequuntur id, eos ducimus
                voluptates molestiae at dignissimos fuga. Aperiam assumenda
                asperiores tenetur deleniti facilis explicabo minus optio autem!
                Repellat, qui repellendus! Culpa commodi velit libero, inventore
                optio consectetur itaque totam iste officia, natus odit iure.
                Optio, deleniti quod adipisci fugiat possimus reprehenderit
                deserunt excepturi rerum ipsum debitis. Magnam, error. Vero
                optio suscipit iusto itaque sint dolores culpa soluta laudantium
                nulla, voluptatibus nesciunt consequatur quas reiciendis
                nostrum? Facilis exercitationem repellat ipsam officiis
                molestias quas officia sunt neque, molestiae at aperiam odit
                accusantium praesentium esse ut nulla, unde placeat
                necessitatibus tempore dolorem ad! Necessitatibus, aliquid
                asperiores cum molestiae voluptas nesciunt, suscipit numquam,
                veritatis rerum ex doloribus totam minus ea minima dicta? Qui,
                voluptatem mollitia porro ipsam amet impedit deleniti nihil
                repellat nostrum non molestiae suscipit fugiat doloremque esse
                quod, iure dolor, at perferendis? Sunt deleniti temporibus magni
                neque accusamus. Aliquid eaque vero at quisquam, facilis nisi
                autem sapiente, omnis earum deserunt quis commodi quas. Illo est
                delectus inventore corporis animi quia recusandae natus, aperiam
                pariatur minima placeat eum ratione sapiente nihil error odio
                velit aliquam quasi nemo earum voluptatem! Qui magnam beatae
                vel? Fugit minima molestias ipsum magnam laudantium corporis
                expedita quis ad quasi cumque, enim eos reiciendis, nam
                asperiores nisi iste explicabo odio. Provident necessitatibus
                sed illo, facere nam laboriosam mollitia distinctio ducimus
                perspiciatis laudantium ab. Quas rerum vero ex, minima
                blanditiis nulla quo animi aut porro explicabo sunt quia labore
                nesciunt voluptatibus doloribus officia molestiae veritatis
                doloremque fuga accusamus obcaecati voluptate odio! Ad vel
                inventore assumenda aut labore excepturi ratione! Nostrum
                numquam quas aliquam quo voluptates voluptas veniam labore ipsam
                ullam laudantium corporis laborum obcaecati sit itaque
                voluptatibus tenetur, nulla dolorem possimus, error illo iusto
                adipisci. Totam minima excepturi eligendi, explicabo, aliquam
                molestias tempore rerum aperiam aspernatur exercitationem
                quisquam cumque! Voluptatibus accusamus sed praesentium ipsa
                blanditiis esse nihil, odio iste consequatur temporibus. Quos
                sunt maiores quidem, totam iure recusandae unde labore aliquid
                eveniet suscipit officia nisi nostrum similique dolorum culpa
                corporis? Earum labore reiciendis eum assumenda facilis laborum
                eveniet alias nihil eaque similique, dolorum ipsa id? Cumque
                fugiat rerum eos quasi aliquid minima quisquam ipsam laudantium
                earum nulla eligendi mollitia, ex omnis veritatis corrupti
                necessitatibus ipsum. Laboriosam consequuntur placeat
                voluptatibus sit sequi iure earum quae itaque soluta dignissimos
                possimus molestiae ipsa quos, magnam quas.
            </p>
        </div>

        <div class="col-md-3 ">
            <div class="bg-primary sticky-top my-5  ">
                <div class="">
                    <h3 class="text-center display-5">
                        <strong>Membresia VIP por 30 dias</strong>
                    </h3>

                    <div class="container">
                        <p class="letra2">
                            <li>
                                • Acceso a todas nuestras entradas en telegram
                                con sus patrones en grafica.
                            </li>
                            <li>• Acceso a Mini clases.</li>
                            <li>
                                • Explicacion de las entradas y movimiento
                                importante de BTC.
                            </li>
                            <li>
                                • Llamada grupal en caso de que el mercado lo
                                amerite.
                            </li>
                        </p>
                    </div>
                    <div class="container">
                        <div class="row ">
                            <div class="col text-end my-auto">
                                <h3>20.00 Usd</h3>
                            </div>
                            <div class="col">
                                <a
                                    href="https://t.me/criptoaprendebot"
                                    target="_blank"
                                    class="btn btn-danger btn-block px-5"
                                    style="font-size: 2rem;">Acceder</a
                                >
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
