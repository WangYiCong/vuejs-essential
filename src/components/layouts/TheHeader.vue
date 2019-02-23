<template>
    <header>
        <div class="logo">
            <img src="#" alt="logo">
        </div>
        <div class="navlist">
            <ul class="falist">
                <li v-for="(item,index) in navList" :class="{active: index === activeIndex }">
                    <a href="#" @click="changeIndex(index)">{{item}}</a>
                </li>
            </ul>
        </div>
    </header>
</template>
<script>
export default {
    name: 'TheHeader',
    data(){
        return{
            navList: ['nihao','nihao','nihao','haha','haha'],
            activeIndex: 0
        }
    },
    methods: {
        changeIndex(index){
            this.activeIndex = index;
        }
    }
}
</script>
<style scoped>
    .active{
        font-size: 20px;
        color: white;
        background: green;
    }
</style>


