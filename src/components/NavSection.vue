<template>
    <div class="nav-wrap ">
        <div class="nav flex f-j-s f-a-c">
            <img  class=" nav-logo" src="../assets/logo.png">
            <ul class="nav-link flex">
                <li class="title active">
                    <a href="#mission" style="outline: none;"><span>项目</span></a>
                </li>
                <li class="title">
                    <a href="#mission" style="outline: none;"><span>说明</span></a>
                </li>
                <li class="title">
                    <a href="#mission" style="outline: none;"><span>项目</span></a>
                </li>
                <li class="title">
                    <a href="#mission" style="outline: none;"><span>项目</span></a>
                </li>

                <li class="title">
                    <a href="javascript:void(0)" ><span>EN</span></a>
                </li>
            </ul>
        </div>

    </div>
</template>

<script>
    export default {
        name: 'nav',
        props: {
            msg: String
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less" scoped>
    .fl{
        float: left;
    }
    .fr{
        float: right;
    }
    .nav-wrap{
        width: 100%;
        position: fixed;
        top:0;
        left: 0;
    }
    .nav{
        max-width: 1000px;
        margin: 0 auto;
        height: 100px;
    }
    .nav-logo{
        width: 100px;
        margin-left: 20px;
    }
    .nav-link{
        font-size: 16px;
        color: #ccc;
        .active{
            color: #444 !important;
            /*border-bottom: 2px solid #000;*/
            span {
                display: inline-block;
                box-shadow: 0 2px 0 0 #444444;
            }
        }
        .title{
            /*padding:20px;*/
            a{
                display: inline-block;
                padding-left: 14px;
                padding-right: 14px;
            }

            &:hover{
                .active
             }
        }

    }


</style>
