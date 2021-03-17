<template>
    <div class="box">
        <el-card :body-style="{ padding: '0px' }">
            <el-image :src="src">
                <template #placeholder>
                    <div class="image-slot">
                        加载中<span class="dot">...</span>
                    </div>
                </template>
            </el-image>
            <div style="padding: 14px;">
                <div class="en_div">{{daily_en}}</div>
                <div class="ch_div">{{daily_ch}}</div>
            </div>
        </el-card>
    </div>

</template>

<script>
// import bus from '../common/bus';
export default {
    name: "dashboard",
    data() {
        return {
            src: 'https://cube.elemecdn.com/6/94/4d3ea53c084bad6931a56d5158a48jpeg.jpeg',
            daily_en: 'The early bird get the worm',
            daily_ch: '早起的鸟儿有食吃'
        };
    },
    components: {
    },
    computed: {
    },

    methods: {
    },
};
</script>

<style scoped>

    .en_div {
        font-size: 36px;
        line-height: 42px;
    }

    .ch_div {
        margin-top: 16px;
        font-size: 24px;
        line-height: 30px;
    }

</style>
