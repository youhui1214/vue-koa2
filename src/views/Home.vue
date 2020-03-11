<template>
    <div class="home">
        <div class="left">
            <div class="lt-title">数据结构与算法 相关的文章:</div>
            <div class="lt-wrap">
                <ArticleInfo></ArticleInfo>
                <ArticleInfo></ArticleInfo>
                <ArticleInfo></ArticleInfo>
                <ArticleInfo></ArticleInfo>
            </div>
        </div>
        <div class="right">
            <ArticleAuthor></ArticleAuthor>
        </div>
    </div>
</template>

<script>
import ArticleInfo from '@/components/ArticleInfo.vue';
import ArticleAuthor from '@/components/ArticleAuthor.vue';

export default {
    name: 'Home',
    components: {
        ArticleInfo,
        ArticleAuthor,
    },
    data() {
        return {
            avatar: 'https://fuss10.elemecdn.com/e/5d/4a731a90594a4af544c0c25941171jpeg.jpeg',
        };
    },
};
</script>

<style lang="less" scoped>
    .home {
        margin-top: 60px;
        display: flex;
        .left {
            flex: 1;
            padding: 10px;
            .lt-title {
                font-size: 18px;
                font-weight: bold;
                margin: 20px 0;
            }
            .lt-wrap {}
        }
        .right {
            width: 400px;
            padding: 20px;
        }
    }

</style>
