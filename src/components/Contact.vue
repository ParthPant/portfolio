<template>
    <div class="card h-screen">
        <div class="card-body place-content-center">
            <h1 class="card-title text-[2em] md:text-[3em] mb-10">Get In Touch.</h1>
            <div class="flex flex-col justify-around md:flex-row">
                <div class="card bg-base-100 drop-shadow-lg md:w-[50%] w-full">
                    <form class="card-body form-control">
                        <h1>Send a Message</h1>
                        <input type="text" placeholder="Name" class="my-3 input input-primary input-bordered">
                        <input type="text" placeholder="Email" class="my-3 input input-primary input-bordered">
                        <textarea class="my-3 textarea h-24 textarea-bordered textarea-secondary" placeholder="Message"></textarea>
                        <input type="submit" class="btn btn-md btn-success my-3" value="Send">
                    </form>
                </div>
                <div class="flex flex-row md:flex-col flex-wrap place-content-center justify-evenly mt-4">
                    <a v-for="link in links" :href="link[1]" :key="link[0]"
                    class="btn btn-md m-2 w-48 gap-x-4 justify-start">
                        <span class="w-7">
                            <fa :icon="['fab', link[0]]" size="2x"/>
                        </span>
                        <div class="w-[1px] bg-white h-8"></div>
                        <p class="">{{ link[0] }}</p>
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    data: function() {
        return {
            links: [
                ['linkedin', 'https://www.linkedin.com/in/parth-pant-866bb4189/'],
                ['github', 'https://www.github.com/ParthPant'],
                ['twitter', 'https://www.twitter.com/PantParth'],
                ['instagram', 'https://www.instagram.com/pantparth'],
            ]
        }
    }
}

</script>


<style scoped>

</style>
