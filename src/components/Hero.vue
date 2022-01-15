<template>
    <div class="items-center justify-evenly md:justify-around flex lg:flex-row flex-col-reverse h-screen">
        <div class="text-white flex flex-col">
            <div class="font-medium sm:text-[2em] text-[3em] md:mt-5 lg:mt-0">Hi! I'm</div>
            <div class="lg:text-[7em] text-[4em] font-bold">{{ name }}.</div>
            <div class="btn btn-outline">Software Developer</div>
        </div>

        <div class="avatar lg:mt-5 md:mt-10">
          <div class="rounded-full drop-shadow-xl sm:w-96 sm:h-96 w-60 h-60">
            <img src="../assets/dp.jpeg">
          </div>
        </div> 
    </div>
</template>

<script>
export default {
    data() {
        return {
            name: 'Parth Pant',
        }
    }
}
</script>

<style scoped>
</style>
