<template>
    <footer class="page-footer font-small mt-3 mb-0 text-left">
        <ul v-for="name in names" :key="name">
            <li><a href="" style="color:black;">{{ name }}</a></li>
        </ul>
    </footer>
</template>

<script lang="ts">
export default ({
    data(){
        return{
            names: ["terms of service", "privacy policy", "iphone app", "android app", "users", "collections", "Explore"],
            links: ["a"]
        }
    }
})
</script>

<style scoped>
footer{
    position: relative;
    top: 200px;
    display: inline;
    height: 100px;
    padding-top: ;
    left: 0;
    bottom: 0;
    width: 100%;
    text-align: center;
}
ul {
    list-style-type: none;
    display: inline;
}
li {
    display: inline;
    
}
a{
    color: black;
    font-weight: bold;
}
</style>
