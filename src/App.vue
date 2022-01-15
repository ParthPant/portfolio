<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import Hero from './components/Hero.vue'
import Menu from './components/Menu.vue'
import About from './components/About.vue'
import Work from './components/Work.vue'
import Contact from './components/Contact.vue'
</script>

<template>
    <div class="bg-grid-pattern h-full">
        <Menu>
            <Hero/>
            <About/>
            <Work/>
            <Contact/>
        </Menu>
    </div>
</template>

<style>
#app {
  height: 100vh;
}
</style>
