<template>
    <div class="nav">
        <el-menu :default-active="activeIndex" class="el-menu-demo" router="true" mode="horizontal" @select="handleSelect">
            <el-menu-item index="1" route="/article">首页</el-menu-item>
            <el-menu-item index="2">项目</el-menu-item>
            <el-menu-item index="3">留言</el-menu-item>
            <el-menu-item index="4" route="/about">关于</el-menu-item>
        </el-menu>
    </div>
</template>

<script>
export default {
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
        margin: 0 200px;
    }

</style>
