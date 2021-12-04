<template>
    <div id="app">
        <h1>Fetch data with API</h1>
        <EmployeeList />
    </div>
</template>
<script>
    import EmployeeList from './components/EmployeeList'
    export default {
        name:"App",
        comments: {
            EmployeeList
        }
    };
</script>

<style>
    #app{
        font-family: Phetsarath OT, Times New Roman;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>