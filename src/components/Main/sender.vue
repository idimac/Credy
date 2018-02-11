<template>
<div>
    <p v-for="text in receivedData" :key="text.id" v-html="text.text"></p>
    <button v-on:click="receivingData">Push me</button>
</div>
</template>
<script>
    import axios from "axios";
    import VueAxios from "vue-axios";
    export default {
        name: 'sender',
        props: ['url'],
        data () {
            return {
                receivedData: []
            }
        },
        methods: {
            receivingData: function () {
                    axios.get(this.url).then((response) => {
                        this.receivedData = response.data;
                        this.$emit('receivedData', this.receivedData);
                    });
                     
                    
            }
        },
        components: {
            "axios": axios,
            "VueAxios": VueAxios,
        }

    }



</script>
<style>
</style>