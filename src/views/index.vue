<template>
    <div>
        <header class="header">
            <row>
                <i-col span="4" class="textCenter">
                    <img class="headerLogo" src="@/assets/index/logo.png">
                </i-col>
                <i-col span="20" class="fl">
                    <ul class="nav">
                        <li class="fl">首页</li>
                        <li class="fl" @click="jump('#demos')">作品展示</li>
                        <li class="fl">解决方案</li>
                        <li class="fl">联系我们</li>
                    </ul>
                </i-col>
            </row>
        </header>
        <div class="section1">
            <row>
                <i-col span="10" offset="2">
                    <img class="img-responsive" src="@/assets/index/section1.png">
                </i-col>
                <i-col span="10">
                    <div class="section1Detail">
                        <p>
                            <img class="section1Logo" src="@/assets/index/sectionLogo.png">
                        </p>
                        <span class="titleLine"></span>
                    </div>
                </i-col>
            </row>
        </div>
        <div>
            <h2 id="demos">作品集</h2>
        </div>
        <div>

        </div>
        <footer>

        </footer>
    </div>
</template>

<script>
export default {
    name: 'index',
    methods: {
        jump(str) {
            document.querySelector(str).scrollIntoView(true);
        }
    }
}
</script>

<style lang="scss" scoped>
.img-responsive {
  display: inline-block;
  height: auto;
  max-width: 100%;
}
.header{
    padding-top: 14px; 
    .headerLogo{
        width: 152px;
        height: 64px;
    }
    .nav{
        height: 69px;
        li{
            height: 69px;
            font-size: 14px;
            font-family: Arial;
            font-weight: 400;
            line-height: 69px;
            color: #232323;
            padding-left: 35px;
        }
    }
}
.section1{
    padding: 60px 0 100px;
    .section1Detail{
        margin: 120px 0 0 85px;
        .sectionLogo{
            width: 100px;
            height: 30px;
        }
        .titleLine{
            display: block;
            width: 100px;
            height: 2px;
            border-bottom: 2px solid #000; 
        }
    }
}
</style>
