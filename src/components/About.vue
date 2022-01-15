<template>
    <div class="card h-screen">
        <div class="card-body place-content-center">
            <h1 class="card-title text-[2em] md:text-[3em] mb-10">About Me</h1>
            <p>{{ about }}</p>
            <div class="flex gap-x-10 flex-wrap my-4">
                <div v-for="skill in skills" :data-tip="skill[0]" class="tooltip" :key="skill">
                    <fa :icon="['fab', skill[1]]" size="2x" class="my-4"/>
                </div>
            </div>
            <button class="btn btn-primary md:w-48">Resume</button>
        </div>
    </div>
</template>

<script>

export default {
    data: function () {
        return {
            about: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Quisque imperdiet ac elit a faucibus. Etiam vitae massa augue. Nullam aliquet volutpat ligula, et tristique massa iaculis sed. Integer luctus, dui eu finibus iaculis, odio diam rutrum dui, vitae rhoncus ipsum metus sollicitudin nulla. Aliquam gravida blandit libero, ac vehicula purus porta a. Duis vehicula erat id leo varius, bibendum eleifend arcu ultrices. Duis et auctor metus. Praesent vel sapien eget elit porttitor pretium et vitae lacus. Morbi sit amet eleifend justo.",
            skills: [
                ["Linux", "linux"],
                ["C/C++", "cuttlefish"],
                ["Rust", "rust"],
                // ["HTML", "html5"],
                ["JavaScript & TypeScript", "js"],
                // ["TypeScript", "ts"],
                ["NodeJS", "node"],
                ["Git", "git"],
                ["React", "react"],
                ["Vue", "vuejs"]
            ]
        }
    }
}

</script>

<style>
</style>
