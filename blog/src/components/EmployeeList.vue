<template>
    <div>
        <h1>Employee List</h1>
    </div>
</template>
<script>
    import Vue from 'vue';
    import axios from 'axios'
    import VueAxios from 'vue-axios'
    Vue.use(VueAxios, axios)
    export default {
        name:"EmployeeList",
        mounted() {
            Vue.axios.get('http://dummy.restapiexample.com/api/v1/employees')
            .then((resp)=>{
                console.warn(resp)
            })
        },
    }
</script>