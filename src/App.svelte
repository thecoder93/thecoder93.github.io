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
    <!-- <div class="w-full relative">
      <div class="w-full h-full flex flex-col absolute top-0 left-0 justify-center items-center">
        <div class="text-6xl font-bold text-white">Home</div>
        <div class="text-2xl text-white">Sottotitolo</div>
      </div>
      <img src="src\assets\images\hero-image.jpg" alt="Image alt text" />
    </div>  -->
    <Hero/>

  </Route>
  {#each link as item}
  <Route path={item.path}>
    <Content {item}/>
  </Route>
  {/each}
<Footer/>
</Router>

