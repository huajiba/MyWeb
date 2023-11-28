<script>
    // 导入组件
    import Course from './Course.vue'
    
    export default{
        data(){
            return{
                CourseDataList:[
                    
                    {
                        src:"./src/components/img/project-2.jpg",
                        name:"title2"
                    },
                    {
                        src:"./src/components/img/project-3.jpg",
                        name:"title3"
                    },
                    {
                        src:"./src/components/img/project-4.jpg",
                        name:"title4"
                    },
                ]
            }
        },
        components:{
            // 注册组件
            Course
        }
    }
</script>
<template>
    <div class="container">
        <!--g-4间距-->
        <div class="row g-4">
            <div class="col-lg-3 col-md-6 col-sm-6">
                <course imgSrc="./src/components/img/project-1.jpg" courseName="Title1"></course>
            </div>
            <div class="col-lg-3 col-md-6 col-sm-6" v-for="x in CourseDataList">
                <course :imgSrc="x.src" :courseName="x.name"></course>
            </div>

            <div class="col-lg-3 col-md-6 col-sm-6">
                <course imgSrc="./src/components/img/project-1.jpg" courseName="Title1"></course>
            </div>
            <div class="col-lg-3 col-md-6 col-sm-6" v-for="x in CourseDataList">
                <course :imgSrc="x.src" :courseName="x.name"></course>
            </div>
            
        </div>
    </div>
</template>

<style></style>