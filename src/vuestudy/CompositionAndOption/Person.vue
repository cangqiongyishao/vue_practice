
<script setup name="Person">
//ref
import {ref} from 'vue';

let username=ref('xiao')

let person=ref({
    username:'xiao',
    age:18
})

const onUpdateUsername=() =>{
    username.value='Feng'
}
const onUpdateAge=()=>{
    person.value.age ++;
}

</script>

<template>
    <h1>username:{{ username }}</h1>
    <div>
        <button @click="onUpdateUsername">Change Username</button>
    </div>
    <h1>age:{{ person.age }}</h1>
    <div>
        <button @click="onUpdateAge">Change Age</button>
    </div>

</template>

<style scoped>

</style>