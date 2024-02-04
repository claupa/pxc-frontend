<script lang="ts">
import { defineComponent } from 'vue';

interface MenuItem {
    id: number;
    label: string;
    url: string;
}

export default defineComponent({
    name: 'TopNavBar',
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
    <footer id="fh5co-footer">

        <div class="container">
            <div class="row row-padded">
                <p class="fh5co-social-icons">
                    <a href="#">
                        <i class="icon-twitter"></i>
                    </a>
                    <a href="#">
                        <i class="icon-facebook"></i>
                    </a>
                    <a href="#">
                        <i class="icon-instagram"></i>
                    </a>
                    <a href="#">
                        <i class="icon-dribbble"></i>
                    </a>
                    <a href="#">
                        <i class="icon-youtube"></i>
                    </a>
                </p>
                <p>
                    <span id="footer-information">11 000 000 pixels sold
                        <br class="hidden">
                        11 000 000 available pixels</span>
                    <small>&copy; Pixel Cubano 2024.
                        <br class="hidden"> All Rights Reserved'.</small>
                </p>
            </div>
        </div>
    </footer>
</template>
