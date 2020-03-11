<template>
    <div class="home">
        <!--<img alt="Vue logo" src="../assets/logo.png">-->
        <Nav></Nav>
        <div class="line"></div>
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
    .home {
        /*margin: 0 200px;*/
    }

</style>
