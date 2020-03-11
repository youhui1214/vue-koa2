<template>
    <div class="main">
        <div class="lt-section">
            <div class="lt-section-left">
                <div class="lt-section-left-title">
                    JavaScript 数据结构与算法之美 - 桶排序、计数排序、基数排序
                </div>
                <div class="lt-section-left-content">
                    笔者写的 JavaScript 数据结构与算法之美
                    系列用的语言是 JavaScript ，旨在入门数据结构与算法和方便以后复习。
                    之所以把 计数排序、桶排序、基数排序 放在一起比较，是因为它们的平均时间复杂度都为 O(n)。
                </div>
                <div class="lt-section-left-info">
                    <span class="info-num">查看 1445</span>
                    <span class="info-num">评论 17</span>
                    <span class="info-num">赞 5</span>
                    <span class="info-time">2019-07-30 22:25:15</span>
                </div>
            </div>
            <div class="lt-section-right">
                <img :src=avatar alt="title" width="100" height="100">
            </div>
        </div>
        <el-divider></el-divider>
    </div>
</template>

<script>
export default {
    name: 'ArticleInfo',
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
        .lt-section {
            display: flex;
            flex-direction: row;
            justify-content: center;
            align-items: center;
            .lt-section-left {
                padding-right: 10px;
                .lt-section-left-title {
                    font-size: 18px;
                    font-weight: 700;
                    line-height: 1.5;
                    margin-bottom: 5px;
                }
                .lt-section-left-content {
                    min-height: 30px;
                    margin: 0 0 8px;
                    font-size: 13px;
                    line-height: 24px;
                    color: #555;
                }
                .lt-section-left-info {
                    font-size: 12px;
                    font-weight: 400;
                    line-height: 20px;
                    color: #555;
                    .info-num {
                        margin-right: 15px;
                    }
                }
            }
        }
    }

</style>
