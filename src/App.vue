<template>
    <div id="app">
        <Nav></Nav>
        <div class="app-main">
            <router-view/>
        </div>
    </div>
</template>
<script>

import Nav from '@/components/Nav.vue';

export default {
    name: 'Home',
    components: {
        Nav,
    },
};
</script>
<style lang="less">
    #app {
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        color: #2c3e50;
        .app-main {
            margin: 0 auto;
            width: 1200px;
        }
    }
</style>
