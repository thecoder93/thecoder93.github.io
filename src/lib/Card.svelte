<script>
    export let title
    export let body
    export let tag = []

</script>
<!-- <div class="max-w-sm rounded overflow-hidden shadow-lg bg-white m-6">
    <div class="px-6 py-4">
      <div class="font-bold text-xl mb-2">{title}</div>
      <p class="text-gray-700 text-base">
        {body}
      </p>
    </div>
    <div class="px-6 pt-4 pb-2">
        {#each tag as item}
            <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">{item.title}</span>
        {/each}
    </div>
  </div>
 -->


  <div class="my-20">
    <div class="max-w-sm rounded-lg border border-gray-200 bg-white shadow-lg m-6">
      <div class="text-right p-4">
        <span class="text-xs text-gray-500 tracking-widest uppercase">{title}</span>
      </div>
  
      <div class="flex items-center relative mb-10">
        <div class="border-t border-gray-200 z-20 w-full"></div>
  
        <div class="rounded-full bg-red-400 z-30 p-2 inline-block absolute mx-8">
          <svg class="fill-current text-white inline-block h-10 w-10" height="72" viewBox="0 0 72 72" width="72" xmlns="http://www.w3.org/2000/svg">
            <path d="M24.0624545,22.6532727 C26.4559091,22.6532727
                     28.4607273,20.7771818 28.4607273,18.3185455
                     C28.4607273,15.8615455 26.4559091,13.986
                     24.0624545,13.986 C21.669,13.986 19.6644545,15.8615455
                     19.6644545,18.3185455 C19.6644545,20.7771818
                     21.669,22.6532727 24.0624545,22.6532727
                     L24.0624545,22.6532727 Z M14.9424545,45.8620909
                     C14.6841818,46.9617273 14.5543636,48.1491818
                     14.5543636,49.1179091 C14.5543636,52.9347273
                     16.6240909,55.4686364 21.0226364,55.4686364
                     C24.6706364,55.4686364 27.6278182,53.3020909
                     29.757,49.8043636 L28.4569091,55.0224545
                     L35.7005455,55.0224545 L39.8405455,38.4177273
                     C40.8752727,34.2133636 42.8803636,32.0312727
                     45.9207273,32.0312727 C48.3139091,32.0312727
                     49.8016364,33.5195455 49.8016364,35.9765455
                     C49.8016364,36.6886364 49.7367273,37.464
                     49.4781818,38.3050909 L47.3432727,45.9373636
                     C47.0198182,47.037 46.8910909,48.1374545
                     46.8910909,49.1713636 C46.8910909,52.7948182
                     49.0251818,55.4451818 53.4880909,55.4451818
                     C57.3043636,55.4451818 60.3441818,52.9884545
                     62.0260909,47.1021818 L59.1804545,46.0033636
                     C57.7570909,49.947 56.5281818,50.6599091
                     55.5580909,50.6599091 C54.5877273,50.6599091
                     54.0700909,50.0135455 54.0700909,48.7205455
                     C54.0700909,48.1385455 54.1999091,47.4924545
                     54.3935455,46.7146364 L56.4638182,39.2787273
                     C56.9809091,37.5327273 57.1753636,35.9844545
                     57.1753636,34.5619091 C57.1753636,28.9993636
                     53.8115455,26.0964545 49.7367273,26.0964545
                     C45.9207273,26.0964545 42.0395455,29.5385455
                     40.0996364,33.1611818 L41.5221818,26.6588182
                     L30.462,26.6588182 L28.9093636,32.3860909 L34.0840909,32.3860909
                     L30.8978182,45.1437273 C28.3952727,50.7062727 23.7987273,50.7965455
                     23.2219091,50.6672727 C22.2747273,50.4537273 21.669,50.094 21.669,48.8631818
                     C21.669,48.153 21.7982727,47.133 22.1217273,45.903 L26.9732727,26.6588182
                     L14.6841818,26.6588182 L13.1315455,32.3860909 L18.2410909,32.3860909 L14.9424545,45.8620909
                     L14.9424545,45.8620909 Z"></path>
          </svg>
        </div>
      </div>
      <div class="px-8 pb-4">
        <h4 class="text-gray-500 text-sm font-light">InVision</h4>
        <h2 class="text-gray-800 text-xl font-bold">InVision</h2>
        <p class="text-gray-600 text-xs">
            {body}
        </p>
      </div>
      <div class="px-6 pt-4 pb-2">
        {#each tag as item}
            <span class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">{item.title}</span>
        {/each}
    </div>
    </div>
  </div>