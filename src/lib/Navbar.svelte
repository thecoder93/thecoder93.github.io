
<script>
import { link, linkSocial } from "../shared/linkNavbar";

    import Link from "svelte-link";
</script>

<nav class="flex items-center justify-between flex-wrap bg-purple-700 p-6 bg-gradient-to-r from-indigo-500 ">
  <div class="flex items-center flex-shrink-0 text-white mr-6">
  
    <!-- <svg class="fill-current h-8 w-8 mr-2" width="54" height="54" viewBox="0 0 54 54" xmlns="http://www.w3.org/2000/svg"><path d="M13.5 22.1c1.8-7.2 6.3-10.8 13.5-10.8 10.8 0 12.15 8.1 17.55 9.45 3.6.9 6.75-.45 9.45-4.05-1.8 7.2-6.3 10.8-13.5 10.8-10.8 0-12.15-8.1-17.55-9.45-3.6-.9-6.75.45-9.45 4.05zM0 38.3c1.8-7.2 6.3-10.8 13.5-10.8 10.8 0 12.15 8.1 17.55 9.45 3.6.9 6.75-.45 9.45-4.05-1.8 7.2-6.3 10.8-13.5 10.8-10.8 0-12.15-8.1-17.55-9.45-3.6-.9-6.75.45-9.45 4.05z"/></svg> -->
    <Link href="/"><span class="font-semibold text-xl tracking-tight">Gianluca La Manna</span></Link>
  </div>
  <div class="block lg:hidden">
    <button class="flex items-center px-3 py-2 border rounded text-teal-200 border-teal-400 hover:text-white hover:border-white">
      <svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/></svg>
    </button>
  </div>
  <div class="w-full block flex-grow lg:flex lg:items-center lg:w-auto">
    <div class="text-sm lg:flex-grow">
      {#each link as item}
      <Link href={item.path} class="block mt-4 lg:inline-block lg:mt-0 text-stone-50 hover:text-white mr-4">{item.title}</Link>
      {/each}
      
    </div>
    <div>
      {#each linkSocial as item}
      
      <a href={item.url} type="button" title={item.title} class="rounded-full border-2 border-white text-white leading-normal uppercase hover:bg-black hover:bg-opacity-5 focus:outline-none focus:ring-0 transition duration-150 ease-in-out w-9 h-9 m-1">
        {@html item.svg}
      </a>
      {/each}
    </div>
  </div>
</nav>