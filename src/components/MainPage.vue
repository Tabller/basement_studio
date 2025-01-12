<script setup>
import { ref } from 'vue'

defineProps({
    msg: String,

})

</script>

<template>
    <h1>{{ msg }}</h1>
    <div class="card">
        <p class="small_Text">There is so much to be done!</p>
    </div>
</template>

<style scoped>
.small_Text{
    color: #888;
}
</style>