<template>
    <div class="goods">
        <ul>
            <li v-for="(item,index) in goodsList" :key="item.id">
                <div class="goods-top">
                    <img :src="item.imgUrl" alt="" />
                    <div class="goods-icon">
                        <img class="left" :src="item.leftUrl" alt="" />
                        <img class="right" :src="item.rightUrl" alt="" />
                    </div>
                    <div class="goods-actor">
                        <img :src="item.actor" alt="" />
                        <span class="actornaame">{{ item.actorname }}</span>
                        <span class="actortag">{{ item.actortag }}</span>
                    </div>
                </div>
                <div class="goods-bottom">
                    <h3>{{ item.name }}</h3>
                    <div class="price">
                        <span class="fuhao">￥</span>
                        <span class="jine">{{ item.price }}</span>
                        <span class="baoyou">
                            <img :src="item.byUrl" alt="" />
                        </span>
                        <span class="xiaoliang">销量999</span>
                    </div>
                </div>
            </li>
        </ul>
    </div>
</template>

<script setup>
    let goodsList=[{
        id:1,
        name:'甜美各式的小夹子',
        actor:'./image/s-1.webp',
        actorname:'小甜心',
        actortag:'爆单女王',
        price:'199',
        sales:500,
        imgUrl:'./images/s-1.webp',
        leftUrl:'./images/zhibotongjia.png',
        rightUrl:'./images/zhibo.png',
        byUrl:'./images/baoyou.png'
    }]
</script>

<style scoped>
    .goods ul li .goods-top .goods-actor .actortag{
        font-size:0.3rem;
        padding: 0 0.125rem;
        background-color: rgba(0,0,0,.5);
        color: white;
        border-radius: 0.0625rem;
    }
    .goods ul li .goods-bottom{
        width:100%;
        padding: 0.1875rem;
        box-sizing: border-box;
    }
    .goods ul li .goods-bottom h3{
        font-size: 0.359rem;
        font-weight: 100;
    }
    .goods ul li .goods-bottom .price{
        width: 100%;
        height:0.625rem;
        position: relative;
        margin-top: 0.3125rem;
    }
    .goods ul li .goods-bottom .price .fuhao{
        font-size:0.375rem;
        color:#f46;
    }







    /*-----------*/
    .goods ul li .goods-top .goods-actor{
        position: absolute;
        bottom: 0;
        left:0;
        width:100%;
        height:0.9375rem;
        padding:0 0 0 0.3125rem;
        display: flex;
        align-items: center;
        box-sizing: border-box;
    }
    .goods ul li .goods-top .goods-actor img{
        width:0.6rem;
        height:0.6rem;
        
    }








</style>