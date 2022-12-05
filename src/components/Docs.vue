<template>
    <div>
        <h1>DocExpire</h1>
        <div v-for="item in items" v-bind:key="item.id">
        <h3>{{item.name}}</h3>
        <p>{{item.exp}}</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: "DocsVue",
        props: ["items"]
    }
</script>

<style scoped>

</style>
