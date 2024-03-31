<h1>Angie!</h1>
<p>This is a nice dinosaur. His name is Fred. Whatever you do, don't click the button!</p>
<script>
    import Card from "./Card.svelte";
    import Something from "./Something.svelte";
    
    let src = "/images/dino.png";
    let msg = "Don't click me!"
    // Select the button by its ID
    function dino(){
        src = "/images/dino.png";
        msg = "Don't click me!"
    }
    
    function dinoRawr(){
        src = "/images/dino-rawr.png";
        msg = "RAWR!!!"
    }
</script>


<img style="width: 10%; height: auto;" {src} />

<br/><br/><br/>

<button on:mousedown={dinoRawr} on:mouseup={dino}>{msg}</button>
