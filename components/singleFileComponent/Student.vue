<!-- 结构 -->
<template>
    <!-- 准备好一个容器 -->
    <div id="root">
        <h2>学生姓名{{studentName}}</h2>
        <h2>学生年龄：{{age}}</h2>
        <button @click="getStudentName()">点我获取学生姓名</button>
    </div>

</template>



<!-- 交互 -->
<script>
export default{
    // 制定组件的名称
    name:'Student',
    data() {
        return {
            studentName: 'misteryliu',
            age: 18
        }
    },
    methods: {
        getStudentName(){
            alert('学生的名字是'+this.studentName)
        }
    }
}
</script>


<style>
.root{
    background-color: red;
}

</style>