<template>
    <div id="Header">
        <!-- 免费咨询 -->
        <div class="top-left-edition">
      <span style="color:#21b3b9;font-weight:bold;">
        <i class="el-icon-phone-outline" style="font-size:23px;"></i>免费咨询：010-12345678
      </span>
            <span>
        <i class="el-icon-time" style="font-size:23px;"></i>工作时间：8:00-18:00
      </span>
        </div>
        <!-- CT图像处理字（可删除放图片） -->
        <div id="word">

            <h1>{{msg}}</h1>
        </div>
    </div>
</template>
<script>
    export default {
        name: "Header",
        data() {
            return {
                msg: "肿瘤辅助诊断系统",
                activeIndex: "1"
            };
        },
        methods: {
            handleSelect(key, keyPath) {
                console.log(key, keyPath);
            }
        }
    };
</script>
<style scoped>
    #Header {
        padding: 30px 110px 0 150px;
        width: 90%;
        margin: 10px auto;
    }

    #word {
        margin-left: 45%;
        margin-top: -35px;
        margin-bottom: 37px;
        height: 60px;
        /* box-shadow: 0 2px 4px rgba(0, 0, 0, 0.12), 0 0 6px rgba(0, 0, 0, 0.04); */
        line-height: 3.2em;
    }

    h1 {
        /*text-align: center;*/
        color: #21b3b9;
        letter-spacing: 30px;
        font-size: 2.3em;
    }

    .el-menu-demo {
        width: 80%;
        margin: 0px auto;
        padding: 0px auto;
    }

    .top-left-edition span i {
        float: left;
        margin-right: 10px;
    }

    i,
    input,
    label {
        vertical-align: middle;
    }

    i {
        border: 0;
        display: block;
        cursor: pointer;
    }

    .top-left-edition span {
        float: left;
        font-size: 16px;
        color: #999999;
        line-height: 24px;
        margin-right: 40px;
    }
</style>


