<script>
  import {Router, Route} from 'svelte-routing'
import Footer from './lib/Footer.svelte';
import Navbar from './lib/Navbar.svelte';
import { link } from './shared/linkNavbar';

</script>

<Router>
  <Navbar/>
  <Route path="/">
    Home
  </Route>
  {#each link as item}
  <Route path={item.path}>
    {item.title}  
  </Route>
  {/each}
<Footer/>
</Router>

