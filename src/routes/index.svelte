<script>

    let text = "Learning svelte for personal use"

    const click_to_change = () => {
        console.log("CLicked me to changed the text");
        text = "I'm being changed cuz you chose to change the text'"
    }

    const click_to_back = () => {
        console.log("CLicked me to back the text");
        text = "Learning svelte for personal use"
    }

</script>

<svelte:head>
    <title>LEARNING SVELTE</title>
</svelte:head>




<h1> {text} </h1>
<div class="container">
<button on:click={click_to_change} class="click-me-button">
Click me to Change
</button>
<button on:click={click_to_back} class="click-me-button">
    Click me to Back
    </button>
</div>
<style>
  
    h1 {
        text-align: center;
        font-size: 49px;
        font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        /* text-decoration: line-through #fff 5px; */
        padding-top: 2.5em;
        padding-bottom: 2.5em;
        padding-left: 3em;
        padding-right: 3em;
        margin-top: 0.5em;
        background-color: cornflowerblue;
    }
  .container {
      display: flex;
      justify-content: center;
      align-items: center;
      /* background-color:aquamarine */
  } 
  .click-me-button{
        padding: 0.75em;
        margin: 0.75em;
        display: flex;
        justify-content: center;
        align-items: center;
        border: 1px solid black;
        border-radius: 0.5em;
        background-color: aquamarine;
        font-weight: bold;
    }
</style>
