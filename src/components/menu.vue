<template>

    <div class="menu-box">
        <ul>
            <li @click="toFrontEnd" @mouseover="onFrontEnd">前端开发</li>
            <li @click="toBackEnd" @mouseover="">后端开发</li>
            <li @click="toFrontEnd">移动开发</li>
            <li @click="toFrontEnd">数据库</li>
            <li @click="toFrontEnd">云计算&大数据</li>
            <li @click="toFrontEnd">运维&测试</li>
            <li @click="toFrontEnd">UI设计</li>
        </ul>
        <div v-show="isFrontEnd" class="inner"></div>
    </div>


</template>

<script>
    export default {
        data(){
            return {
                isFrontEnd:false
            }
        },
        methods: {
            onFrontEnd(){
                this.isFrontEnd = true
            },
            toFrontEnd(){
                alert('跳转到前端')
            },
            toBackEnd(){
                alert('跳转到后端')
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .menu-box {
        width: 216px;
        height: 444px;
        padding-top: 12px;
        background: #2b333b;
        border-bottom-left-radius: 0.5rem;
        border-top-left-radius: 0.5rem;
        float: left;
        position: relative;

    }

    ul {
        margin: 0;
        padding: 0;
    }

    li {
        padding: 20px;
        margin-left: 10px;
        color: rgba(255, 255, 255, .3);
        border-bottom-left-radius: 0.5rem;
        border-top-left-radius: 0.5rem;
        font-weight: 1000;
        list-style: none;
    }

    li:hover {
        color: white;
        background-color: rgba(255, 255, 255, .6);
        cursor: pointer;
    }
    li:hover .inner{
        opacity: 1;
    }

    .inner {
        width: 768px;
        height: 210px;
        background-color: black;
        position: absolute;
        float: left;
        left: 216px;
        top:0;
        opacity: 1;
    }

</style>