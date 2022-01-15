<template>

<div class="min-h-screen card">
    <div class="place-content-center card-body">
        <h1 class="card-title text-[2em] md:text-[3em] mb-10">Projects & Internships</h1>
        <div v-for="project in projects" :key="project.name" class="card card-bordered my-8 bg-base-100 drop-shadow-md">
            <div class="card-body">
                <h1 class="card-title">{{ project.name }}</h1>
                <div class="flex flex-wrap gap-x-5 my-3">
                    <div v-for="tag in project.tags" :key="tag" class="badge
                    badge-primary" :style="getStyle(tag)">{{ tag }}</div>
                </div>
                <p>{{ project.desc }}</p>
                <div class="card-actions">
                    <a v-for="(value, name, idx) in project.link" :key="idx" :href="value" class="btn btn-sm btn-accent btn-outline">{{ name }}</a>
                </div>
            </div>
        </div>
    </div>
</div>

</template>

<script>
import projects from "../data/projects.json"

export default {
    methods: {
        getStyle(tag) {
            return {
                "background-color" : this.colors[tag],
                "border-color" : this.colors[tag]
            }
        }
    },
    data: function () {
        return {
            projects,
            colors: {
                "web" : "magenta",
                "cpp" : "blue",
                "rust": "orange",
                "js"  : "dark-blue",
            }
        }
    }
}
</script>

<style scoped>

</style>

