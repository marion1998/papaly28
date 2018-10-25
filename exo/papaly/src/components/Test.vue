<template>
<div id="test">
    <h3><b>Hey, regarde mon </b> 
    <a href="https://github.com/marion1998" target="_blank" rel="noopener">Github</a>
    </h3>
    <button @click="counter += 1">Increment</button>
    <h1> the button : {{ counter }} </h1>
</div>
</template>

<script>
export default {
    name: 'Test',
    data() {
        return {counter: 0}
    }
}
</script>

