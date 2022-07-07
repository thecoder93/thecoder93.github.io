<script>
import Card from "./Card.svelte";


    export let item

    export let tagCard = [
    {
        title: 'Javascript',
       
    },
    {
        title: 'React',
    },
    {
        title: 'Svelte',
    }
]    

</script>


<div class="w-full relative text-white">
    <div class="bg-indigo-100 font-sans">
      {#if item.title === 'About'}
      <h1 class="text-7xl font-bold	p-9 text-black"> Bio </h1>
            <p class="text-lg p-9 text-black">Da piccolo mi incuriosiva come un Donkey Kong sullo schermo potesse muoversi nelle direzioni in cui io volevo, solo attraverso un joypad. Così nel tempo cercai di capire cosa stava dietro quel mondo. In generale si trattava di programmazione e fu lì che mi appassionai così tanto da intraprendere sia gli studi liceali che universitari nell’ambito informatico.
                Nel tempo mi sono interessato anche allo sviluppo di microcontrollori, tanto da presentare qualcosa alla tesi di laurea.
                
                Oggi la mia carriera ha dato spazio ad un percorso di sviluppo frontend. Mi incuriosiscono le novità e soprattutto le metodologie per produrre del software di qualità.
                
                Quando non sto in sella alla mia Harley, puoi trovarmi alle prese con qualche cotta di birra, o almeno ci sto provando :) Mi piace leggere, soprattutto temi che riguardano la crescita personale.
                Amo viaggiare, pratico Yoga saltuariamente e cerco di mantenermi in forma svolgendo attività in sala fitness.
                D’altronde “Mens sana in corpore sano”. </p>
            <div class="flex justify-center">
                <Card 
                title="Titolo di prova" 
                body="BODY BODY BODY"
                tag={tagCard} />

                <Card 
                title="Titolo di prova" 
                body="BODY BODY BODY"
                tag={tagCard} />

                <Card 
                title="Titolo di prova" 
                body="BODY BODY BODY"
                tag={tagCard} />
        </div>
            
      {/if}
    </div>
  </div> 