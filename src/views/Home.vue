<template>
    <div>
        <ul class="footer">
            <li class="icons"><router-link :to="{name:'list'}">新闻列表</router-link></li>
            <li class="icons"><router-link :to="{name:'user'}">个人中心</router-link></li>
        </ul>
        <router-view />
    </div>
</template>

<script>
    export default {
        name: "Home"
    }
</script>

<style scoped lang="scss">
    *{
        list-style: none;
    }
    .footer{
        position: fixed;
        width: 90%;
        height: 60px;
        line-height: 60px;
        left: 5%;
        bottom: 0;
        display: flex;
        flex-flow: row nowrap;
        justify-content: space-between;
    }
    .icons{
        font-size: 16px;
        flex: 1;
        text-align: center;
        border: 1px solid #42b983;
        a{
            color: #42b983;
            display: block;
            text-decoration: none;
            &.active{
                color: #fff;
                background-color: #42b983;
            }
        }
    }

</style>
