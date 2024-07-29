<template>
  <div>
    <button @click="onUpdateCount">CompositionCnt {{ count }}</button>
  </div>
</template>

<!-- <script>
import {ref} from 'vue'
export default {
    name:'Compositions',
    setup(){
        let count=ref(0);

        function onUpdateCount(){
            count.value +=1
        }
        return {
            count,
            onUpdateCount
        }
    }
}
</script> -->

<!-- <script>
export default {
    name:'Com'
}
</script> -->

<script setup name="Com111">
import {ref} from 'vue'
let count=ref(0);

function onUpdateCount(){
    count.value +=1;
}
</script>

<style>

</style>