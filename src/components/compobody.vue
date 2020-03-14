<template>
    <div class="moibody-container">
        <div class="bodyOne"><h3>{{ msg }}</h3></div>
        <hr>
        <div class="bodyTwo"><p>{{ content }}</p></div>
        <hr>
        <div id="bodyThree">
            <h2>Beach bum? {{ counter }}</h2>
            <button v-on:click="counter++"> Yes  </button>
            <button v-on:click="counter--"> No  </button>
        </div>
    
    </div>    
 
</template>

<script>
export default {
    name: 'compobody',
    props: {
        msg: String,
        content: String,
    data: {
        counter: 0,
    }
              
    }

}
</script>

<style scoped>

    .moibody-container {
        position: fixed;
        left: 0;
        margin: 5px 0px 5px 0;
        width: 100%;
        height: 100vh;
        background-color: #FBBFCA;
        
        text-align: center;

     
    }

    .bodyOne {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-size: 1.5rem;
        text-align: center;
        color: yellow;
    }

    .bodyTwo {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-size: 1.5rem;
        text-align: center;
        color: #F26419;
    }

    .bodyThree {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-size: 2rem;
        text-align: center;
        color: black;
    }

    
</style>