<template>
    <div>
        <h3>{{item.name}}</h3>
        <p>{{item.exp}}</p>
    </div>
</template>

<script>
    export default {
        name:"itemVue",
        props: ["item"]
    }
</script>

<style scoped>

</style>