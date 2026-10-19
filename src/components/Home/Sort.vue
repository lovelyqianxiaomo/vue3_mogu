<template>
    <ul class="sorts">
        <li v-for="(item,index) in sortList" :key="item.id">
            <img :src="item.imgUrl" alt="" />
            <span>{{item.title}}</span>
        </li>
    </ul>  
</template>
<script setup>
    let sortList=[{
        id:1,
        title:'女装',
        imgUrl:'../src/assets/images/nav_01.png'
    },{
        id:2,
        title:'女装',
        imgUrl:'../src/assets/images/nav_02.png'
    },
    {
        id:3,
        title:'女鞋',
        imgUrl:'../src/assets/images/nav_03.png'
    },
    {
        id:4,
        title:'女装',
        imgUrl:'../src/assets/images/nav_04.png'
    },{
        id:5,
        title:'女装',
        imgUrl:'../src/assets/images/nav_05.png'
    },
    {
        id:6,
        title:'女鞋',
        imgUrl:'../src/assets/images/nav_06.png'
    },
    {
        id:7,
        title:'女装',
        imgUrl:'../src/assets/images/nav_07.png'
    },{
        id:8,
        title:'女装',
        imgUrl:'../src/assets/images/nav_08.png'
    },
    {
        id:9,
        title:'女鞋',
        imgUrl:'../src/assets/images/nav_09.png'
    },
    {
        id:10,
        title:'女鞋',
        imgUrl:'../src/assets/images/nav_10.png'
    }]
</script>
<style scoped>
    .sorts {
        width:100%;
        background-color: white;
        font-size:0.35rem;
        box-sizing: border-box;
        display: flex;
        flex-flow:row wrap;
    }

    .sorts li {
        display:flex;
        flex-direction: column;
        align-items: center;
        box-sizing: border-box;
        flex:0 0 20%;
        margin:0.3rem 0;

    }
    .sorts li img{
        width:1.5rem;
        height:1.5rem;
    }
    .sorts li span{
        font-size: 0.38rem;
        color: #000000;
    }
</style>