<script lang="ts">
  import Navbar from "./layout/navbar.svelte";
  import { Router, Route } from "svelte-routing";
  import Home from "./pages/Home.svelte";
  import About from "./pages/About.svelte";
  export const url = "";
</script>

<svelte:head>
  <meta
    name="monetization"
    content="$coil.xrptipbot.com/701298d5-481d-40ff-9945-336671ab2c42" />
</svelte:head>

<Router {url}>
  <Navbar />
  <Route path="/" component={Home} />
  <Route path="/about" component={About} />
</Router>
