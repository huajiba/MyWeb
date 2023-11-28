<script setup>
import Navbar	from './components/Navbar.vue'
import WebIntro from './components/WebIntro.vue'
import Carousel from './components/Carousel.vue'
import CourseListVue from './components/CourseList.vue'
import Father from './components/子传父/Father.vue';
import MySlotVue from './components/MySlot.vue';
</script>

<template>
	<!--
		<Navbar />
		<Navbar></Navbar>
		<navbar></navbar>
	-->
	<!-- <Navbar />
	<WebIntro />
	<Carousel />
	<CourseListVue/> -->
	<!-- <Father/> -->
	<!-- 电商网站案例 -->
	<MySlotVue>
		<button>按钮</button>
	</MySlotVue>
</template>

<style scoped>

</style>
