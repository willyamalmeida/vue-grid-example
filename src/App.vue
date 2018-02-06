<template>
  <div id="app">
    <h4>My example with vue-grid</h4>
    <vue-grid :config="config"></vue-grid>
  </div>
</template>

<script>
import VueGrid from "wa-vue-grid";
//import VueGrid from "./../node_modules/wa-vue-grid/dist/vue-grid";
//import VueGrid from "./../node_modules/wa-vue-grid/src/components/VueGrid.vue";

export default {
    name: "App",

    components: {
        VueGrid
    },

    data() {
        return {
            config: {
                search: 'http://localhost:3000/rows',
                filter: true,
                columns: [
                    {name: 'name', display: 'Name', sort: true},
                    {name: 'email', display: 'E-mail', sort: true}
                ],
                // rows: []
                rows: [
                    { name: "XXX xxx", email: "xxx@xxx.xxx"},
                    { name: "YYY yyy", email: "yyy@yyy.yyy"},
                    { name: "BBB bbb", email: "bbb@bbb.bbb"},
                    { name: "AAA aaa", email: "aaa@aaa.aaa"}
                ]
            }
        };
    }
};
</script>
