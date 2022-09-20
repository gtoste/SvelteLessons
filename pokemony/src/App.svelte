<script>
  import "./index.css"
  import Header from './components/Header.svelte';
  import { Router, Link, Route } from "svelte-navigator";
  import Home from "./routes/Home.svelte";
</script>

<Header />
<div class="w-3/4 m-auto">

  <Router>
    <div>
      <Route path="/">
        <Home />
      </Route>
    </div>
  </Router>
</div>



