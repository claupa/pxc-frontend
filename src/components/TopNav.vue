<script lang="ts">
import { defineComponent } from 'vue';

interface MenuItem {
    id: number;
    label: string;
    url: string;
}

export default defineComponent({
    name: 'Menu',
    data() {
        return {
            menuItems: [
                { id: 1, label: 'Home', url: '/' },
                { id: 2, label: 'About', url: '/about' },
                { id: 3, label: 'Contact', url: '/contact' },
            ] as MenuItem[],
        };
    },
});
</script>

<template>
    <header id="fh5co-header" role="banner">
        <div class="container">
            <div class="row">
                <div class="">
                    <a id="menu" href="#" class="fh5co-menu-btn js-fh5co-menu-btn lowercase m-bold tiny">Menu<i style="padding: 4px 7px 0 7px; margin: 0" class="pxc i-menu"></i></a>
                    <a class="navbar-brand" href="#"> <i id="main-i-logo" class="pxc i-logo"></i></a>		
                </div>
            </div>
        </div>
    </header>
</template>

<style scoped>
nav {
    background-color: #f0f0f0;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    display: inline-block;
    margin-right: 10px;
}

a {
    text-decoration: none;
    color: #333;
}
</style>
