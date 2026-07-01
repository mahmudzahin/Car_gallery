<template>
           <button @click="isOpen = !isOpen" style="text-align: center; align-items: center;">Toggle </button>  
    <div class="container" v-show="isOpen"> 
        <div class="image-wrapper">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSHoMatzsLTTYU9tWd24fbbMrWF-715azpM5VKbe-QeKg&s"
                alt="alion2018">
        </div>
        <div class="card-content">
            <h2>Brand </h2>
            <h3> Allion 2018</h3>
            <p class="description">
                The Toyota Allion 2018 is a highly popular, reliable Japanese mid-size sedan. It is beloved in South
                Asia for its sleek design, luxury features, and excellent fuel efficiency
            </p>
        </div>
        <div class="specification">
            <ul>
                <li>Engine & Peformance  Options
                    <ul style="list-style: none ; display: flex; gap:8px;">
                        <li>1.5L</li>
                        <li>1.8L</li>
                        <li>2.0L</li>
                    </ul>
                </li>
                <li>A15  version</li>
                <li>Generation 2 </li>
                <li>Registration</li>
            </ul>
        </div>

    </div>
</template>

<script setup>

import {ref} from 'vue'

const isOpen  = ref(false);

</script>

<style scoped>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.container {
    width: 300px;
    box-shadow: 4px 8px 12px rgba(0, 0, 0, 0.15);
    display: flex;
    flex-direction: column;
    align-items: center;
    overflow: hidden;
    padding: 8px;
    margin-top: 4px;
}

.image-wrapper {
    width: 100%;
    height: 200px;
}

img {
    width: 100%;
    height: 200px;
    object-fit: cover;
}

.card-content {
    width: 100%;
    display: flex;
    flex-direction: column;
    text-align: center;
    justify-content: center;
    padding: 16px;
    gap:8px;
}

.card-content h2 {
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    font-size: 36px;
    background: linear-gradient(to right, rgb(42, 176, 221), #0a62b9);

    -webkit-background-clip: text;
    background-clip: text;

    /* 3. Make the actual text color transparent so the background shines through */
    color: transparent;
    font-style: italic;
    letter-spacing: 0.2rem;
}

.card-content h3 {
    font-weight: 900;
    font-size: 20px;
    font-style: italic;
}

.card-content p {
    font-size: 15px;
    line-height: 1.2rem;
    letter-spacing: 0.1rem;
}
</style>