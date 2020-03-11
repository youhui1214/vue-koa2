<template>
    <div class="main">
        <div class="rt-user">
            <el-avatar shape="circle" :size="150" :src=avatar></el-avatar>
            <div class="rt-name">呼呼伙伴</div>
        </div>
        <el-divider></el-divider>
        <div class="rt-tag">
            <div class="rt-tag-item"><el-tag type="info">数据结构与算法</el-tag></div>
            <div class="rt-tag-item"><el-tag type="info">JavaScript</el-tag></div>
            <div class="rt-tag-item"><el-tag type="info">vue.js</el-tag></div>
            <div class="rt-tag-item"><el-tag type="info">webpack</el-tag></div>
            <div class="rt-tag-item"><el-tag type="info">你不知道的JavaScript</el-tag></div>
            <div class="rt-tag-item"><el-tag type="info">JavaScript</el-tag></div>
            <div class="rt-tag-item"><el-tag type="info">vue.js</el-tag></div>
            <div class="rt-tag-item"><el-tag type="info">webpack</el-tag></div>
            <div class="rt-tag-item"><el-tag type="info">webpack</el-tag></div>
            <div class="rt-tag-item"><el-tag type="info">webpack</el-tag></div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ArticleAuthor',
    data() {
        return {
            avatar: 'https://fuss10.elemecdn.com/e/5d/4a731a90594a4af544c0c25941171jpeg.jpeg',
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
    .main {
        .rt-user {
            display: flex;
            flex-direction: column;
            align-items: center;
            .rt-name {
                font-family: "Microsoft YaHei","微软雅黑";
                font-size: 22px;
                font-weight: bold;
                margin-top: 20px;
            }
        }
        .rt-tag {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            .rt-tag-item {
                margin: 5px;
            }
        }
    }

</style>
