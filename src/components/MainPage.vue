<script setup>
import { ref } from 'vue'

defineProps({
    msg: String,

})

</script>

<template>
<section class="red">
    <h1>{{ msg }}</h1>
    <div class="card">
        <p class="small_Text">There is so much to be done!</p>
    </div>
    <div class="curve"></div>
</section>
</template>

<style scoped>
section {
    position: top;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 120px 20vw;
    min-height: 400px;
}

.red {
    background-color: #8D021F;
}
.curve {
    position: absolute;
    height: 225px;
    width: 100%;
    bottom: 0%;
}
.curve::before {
    content: '';
    display: block;
    position: absolute;
    border-radius: 100% 50%;
    width: 55%;
    height: 100%;
    background-color: #242424;
    transform: translate(85%, 60%);
}
.curve::after {
    content: '';
    display: block;
    position: absolute;
    border-radius: 100% 39.3%;
    width: 55%;
    height: 100%;
    background-color: #8D021F;
    transform: translate(-2%, 40%);
}
.small_Text{
    color: #888;
}
</style>