<script>
  import {Router, Route} from 'svelte-routing'
import Avatar from './lib/Avatar.svelte';
import Content from './lib/Content.svelte';
import Footer from './lib/Footer.svelte';
import Hero from './lib/Hero.svelte';
import Navbar from './lib/Navbar.svelte';
import { link } from './shared/linkNavbar';

</script>

<Router>
  <Navbar/>
  <Route path="/">
    <Hero/>
  </Route>
  {#each link as item}
  <Route path={item.path}>
    <Content {item}/>
  </Route>
  {/each}
<Footer/>
</Router>

