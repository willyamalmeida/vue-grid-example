<template>
  <div id="app">
    <h1>My example with vue-grid</h1>
    <vue-grid :config="config"></vue-grid>
  </div>
</template>

<script>
import VueGrid from "wa-vue-grid";

export default {
    name: "App",

    components: {
        VueGrid
    },

    data() {
        return {
            config: {
                collumns: [
                    {name: 'Name'},
                    {name: 'Email'}
                ]
            }
        };
    }
};
</script>
