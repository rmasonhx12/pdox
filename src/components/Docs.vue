<template>
    <div>
        <h1>DocExpire</h1>
        <div v-for="item in items" v-bind:key="item.id">
       <!--  <h3>{{item.name}}</h3>
        <p>{{item.exp}}</p> -->
        <Item v-bind:item="item"/>
        </div>
    </div>
</template>

<script>
import Item from './item.vue';
    export default {
        name: "DocsVue",
        props: ["items"],
        components: {
            Item
        }
    }
</script>

<style scoped>

</style>
