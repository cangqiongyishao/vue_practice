<template>
    <div>
        <h1>name:{{ author.username }},age:{{ author.age }}</h1>
        <button @click="onUpdateAuthor">update author</button>
    </div>

    <div>
        <p>book name:{{ books[0].name }},author:{{ books[0].author }}</p>
        <button @click="onUpdateBook">update Book</button>
    </div>
</template>

<script setup>
import { reactive } from 'vue';
let author=reactive({
    username:'Xiao',
    age:200
})

let books=reactive([
    {name:'God and Devil', author:'Xiao'},
    {name:'Dragon on the Sky',author:'Feng'}
])

const onUpdateAuthor=()=>{
    console.log(author.username);
    // author.username='Feng'
    Object.assign(author,{username:'Feng',age:100})
}

const onUpdateBook=()=>{
    // books[0].name='Star faraway'
    Object.assign(books,[
    {name:'Dragon on the Sky',author:'Feng'}
])
}

</script>

<style scoped>

</style>