<template>
    <body>
        <header class="header">
            <div class="header__logo">
                Knowmadmood
            </div>

            <nav class="header__nav">
                <button class="btn btn__primary header__menu"><img src="../assets/images/hamburger_icon_white.svg" alt="menu" width="20" height="auto"></button>
                <button class="btn btn__primary">Login</button>
                <button class="btn btn__primary">Register</button>
            </nav>

        </header>
        <div class="full-grid">
            <aside class="menu">
                <ul>
                    <li>Home</li>
                    <li>About</li>
                    <li>Contact</li>
                </ul>
            </aside>
            <main class="main-page">
                <header class="main-page__header">
                    <h1>Home</h1>
                    <p>Welcome to the home page</p>
                    <nav class="main-page__nav">
                        <button class="btn btn__secondary">All posts</button>
                        <button class="btn btn__secondary">Art</button>
                        <button class="btn btn__secondary">Development</button>
                        <button class="btn btn__secondary">LifeStyle</button>
                        <button class="btn btn__secondary">Accesories</button>
                    </nav>
                </header>
    
                <section class="main-page__content">
                    <h2>Latest Posts</h2>
                    <main class="main-page__grid">
                        <Card v-for="card in numberOfCards" :key="card"></Card>
                    </main>
                </section>
            </main>

        </div>
        <footer class="footer">
            <div class="footer__info">
                © 2024 Knowmadmood
            </div>
        </footer>
  </body>
</template>
  
<script setup>
import Card from '@/components/Card.vue';
const numberOfCards = 5
</script>
  
<style scoped>
</style>