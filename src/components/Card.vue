<template>
    <div class="card">
        <img src="../assets/images/card_img.jpg" alt="card image" class="card__img">
        <section class="card__main">
            <h3>{{ cardContent.title }}</h3>
            <nav class="card__nav">
                <button class="btn btn__primary" v-for="tag in cardContent.tags" :key="tag">{{ tag }}</button>
            </nav>
            <p>{{ cardContent.description }}</p>
        </section>
        <section class="card__bottom">
            <button class="btn btn__secondary">{{ cardContent.cta_text }}</button>
        </section>
    </div>
</template>
  
<script setup>
const cardContent = {
    title: 'Post x',
    tags: ['Art', 'Development'],
    description: 'Lorem ipsum dolor sit amet consectetur',
    cta_text: 'Read more'
}

</script>
  
<style scoped>

</style>