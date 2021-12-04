<template>
    <div>
        <h1>Submit Form Data to API</h1>
        <form @submit="postData" method="post">
            <input type="text" name="author" placeholder="author" v-model="posts.author"> <br /><br />
            <input type="text" name="title" placeholder="title" v-model="posts.title"> <br /><br />
            <button type="submit">Post</button>
        </form>
       
    </div>
</template>
<script>
    import Vue from 'vue';
    import axios from 'axios'
    import VueAxios from 'vue-axios'
    Vue.use(VueAxios, axios)
    export default {
        name:"PostComponent",
        data(){
            return{
                posts:{
                    title:null,
                    author:null
                }
            }

        },
        methods:{
            postData(e){
                this.axios.post("http://localhost:3000/posts/", this.posts);
                //console.warn(this.posts)
                e.preventDefault();
            }
        }
    }
</script>