<script>
  import Senales from "./Senales.svelte";
  import Trading from "./Trading.svelte";
  import Home from "./Home.svelte";
  import { Router, Route, Link, link } from "svelte-routing";
  import Nivel1 from "./Nivel1.svelte";
</script>

<Router>
  <div>
    <Route path="/" component={Home} />
    <Route path="/trading" component={Trading} />
    <Route path="/senales" component={Senales} />
    <Route path="/nivel1/" component={Nivel1} />
  </div>
</Router>
