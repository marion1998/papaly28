<template>
<div id="test">
    <h3><b>Hey, regarde mon </b> 
    <a href="https://github.com/marion1998" rel="noopener">Github</a>
    </h3>
    <h1> {{ msg }} </h1>
    <button v-on:click="sayHello"> sayHello </button>

</div>
</template>

<script>
export default {
    name: "Test",
    props: {
    msg: String
    },
    methods: {
    sayHello: function() {
        let input = document.createElement("input");              //crée un document (de type input)
        input.setAttribute("id", "boardInput");                   //lui donner un id
        document.getElementById("test").appendChild(input);       //aller chercher un document avec son id
        input.addEventListener("keypress", function(e) {
                                                                //ajouter un évènement via des touches
        var key = e.which || e.keyCode;
        if (key === 13) {
                                                                // 13 fait référence à la touche 'Enter'
            let board = document.createElement("div");
            board.setAttribute("id", "board");
            document.getElementById("boardInput").remove();
            
        }
        });
    }
    }
};
</script>
