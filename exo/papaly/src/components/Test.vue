<template>
<div id="test">
    <h3><b>Hey, regarde mon </b> 
    <a href="https://github.com/marion1998" target="_blank" rel="noopener">Github</a>
    </h3>
    <h1> {{ msg }} </h1>
</div>
</template>

<script>
export default {
    name: 'Test',
    props: {
        msg: String
    } 
}
</script>

