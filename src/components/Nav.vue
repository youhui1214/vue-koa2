<template>
    <div class="nav">
        <el-menu :default-active="activeIndex" class="el-menu-demo" router mode="horizontal" @select="handleSelect">
            <el-menu-item index="1" route="/">首页</el-menu-item>
            <el-menu-item index="2" route="/project">项目</el-menu-item>
            <el-menu-item index="3" route="/message">留言</el-menu-item>
            <el-menu-item index="4" route="/about">关于</el-menu-item>
        </el-menu>
    </div>
</template>

<script>
export default {
    name: 'nav',
    data() {
        return {
            activeIndex: '1',
        };
    },
    methods: {
        handleSelect(key, keyPath) {
            console.log(key, keyPath);
        },
    },
};
</script>

<style scoped lang="less">
    .nav {
        width: 100%;
        position: fixed;
        top: 0;
        left: 0;
    }

</style>
