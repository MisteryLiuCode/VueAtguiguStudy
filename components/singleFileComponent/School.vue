<!-- 结构 -->
<template>
    <!-- 准备好一个容器 -->
    <div id="root">
        <h2>学校名称：{{schoolName}}</h2>
        <h2>学校地址：{{address}}</h2>
        <button @click="getSchoolName()">点我获取学校名</button>
    </div>

</template>



<!-- 交互 -->
<script>
export default{
    // 制定组件的名称
    name:'School',
    data() {
        return {
            schoolName:'北京大学',
            address:'北京'
        }
    },
    methods: {
        getSchoolName(){
            alert('学校的名字是'+this.schoolName)
        }
    },
}
</script>


<style>
.root{
    background-color: blue;
}

</style>