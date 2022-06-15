<script>

import { linkSocial } from "../shared/linkNavbar";

</script>
<footer class="text-center bg-gray-900 text-white">
    <div class="container px-6 pt-6 m-auto ">
      <div class="flex justify-center mb-6">
        {#each linkSocial as item}
      
        <a href={item.url} type="button" title={item.title} class="rounded-full border-2 border-white text-white leading-normal uppercase hover:bg-black hover:bg-opacity-5 focus:outline-none focus:ring-0 transition duration-150 ease-in-out w-9 h-9 m-1">
          {@html item.svg}
        </a>
        {/each}
      </div>
  

    <div class="text-center p-4" style="background-color: rgba(0, 0, 0, 0.2);">
      © 2021 Copyright:
      <a class="text-white" href="https://tailwind-elements.com/">Tailwind Elements</a>
    </div>
  </footer>