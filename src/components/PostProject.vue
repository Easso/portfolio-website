<template>
<div><h1>Add new Project</h1></div>
<div class="container">
    <div class="input-container">
        <label for="id">Project Id</label>
        <input type="text" name="id" v-model="postData.projectId">
    </div>
    <div class="input-container">
        <label for="title">Title</label>
        <input type="text" name="title" v-model="postData.title">
    </div>
    <div class="input-container">
        <label for="about">About</label>
        <input type="text" name="about" v-model="postData.about">
    </div>
    <div class="input-container">
        <label for="image">image</label>
        <input type="text" name="image" v-model="postData.image">
    </div>
    <div class="input-container">
        <label for="link1">Link</label>
        <input type="text" name="link1" v-model="postData.link1">
    </div>
    <div class="input-container">
        <label for="link2">Link</label>
        <input type="text" name="link2" v-model="postData.link2">
    </div>

    <button type="submit" @click="PostProject()">Post</button>
</div>
</template>


<script>
import axios from 'axios'
export default {
    data() {
        return {
            postData: {
                projectId: '',
                title: '',
                about: '',
                image: '',
                link1: '',
                link2: ''
            }
        }
    },
    methods: {
        PostProject() {
            axios.post('https://u2mvdypt0e.execute-api.us-east-2.amazonaws.com/production/postprojects', this.postData).then(response => {
                console.log(response)
            }).catch(err => {
                console.log(err)
            }) 
        }
    }
}
</script>

<style>

</style>