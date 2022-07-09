<script>
import Avatar from "./Avatar.svelte";
import sea from "../assets/images/hero-image.jpg";


</script>

<div class="w-full relative">
    <div class="w-full h-full flex flex-col absolute top-8 left-0 justify-center items-center">
        <div class="text-7xl font-bold text-white mt-4">Gianluca La Manna</div>
        <Avatar/>        
      <div class="text-2xl text-white">Frontend Developer @ <a class="underline" href="https://www.flowing.it/">FLOWING</a></div>
      <div class="text-md text-white mt-2"> from Sicily with ♥ </div>

    </div>
    <img src={sea} alt="Tramonto sul mare della Sicilia" />
    
  </div> 