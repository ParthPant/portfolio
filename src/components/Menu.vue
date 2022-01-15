<template>

<div class="drawer drawer-end h-full">
    <input id="my-drawer" type="checkbox" class="drawer-toggle"> 
    <div class="drawer-content ">
        <div class="flex">
            <label for="my-drawer" class="btn btn-square btn-ghost drawer-button fixed right-0 m-4">
                <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="inline-block w-6 h-6 stroke-current">           
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>               
                </svg>
            </label>
        </div>
        <div class="px-10 sm:px-40 lg:px-64">
            <slot>Content</slot>
        </div>
    </div> 

    <div class="drawer-side">
        <label for="my-drawer" class="drawer-overlay"></label> 
        <ul class="menu p-4 overflow-y-auto w-80 bg-base-100 text-base-content text-[2em]">
            <li>
                <a>About</a>
            </li> 
            <li>
                <a>Projects</a>
            </li>
            <li>
                <a>Contact</a>
            </li>
        </ul>
    </div>
</div>

</template>

<script>
export default {
    data() {
        return {
            name: 'Parth Pant'
        }
    }
}
</script>

<style scoped>
</style>
