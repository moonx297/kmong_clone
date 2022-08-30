<template>
	<header id="header">
		<div class="container">
			<section class="sec1">
				<div class="logo-wrap">
					<h1>
						<router-link to="/">
							<img src="@/assets/images/logo.svg" alt="로고" />
						</router-link>
					</h1>
				</div>
				<nav id="nav">
					<el-input
						placeholder="서비스, 전문가를 검색해보세요."
						prefix-icon="el-icon-search"
						v-model="input_search"
					>
					</el-input>
					<router-link to="#">전문가 등록</router-link>
					<router-link to="#1">로그인</router-link>
					<router-link to="#2">무료 회원가입</router-link>
				</nav>
			</section>

			<section class="sec2">
				<div class="nav2">
					<div class="menu-wrap">
						<router-link to="/cate-design">디자인</router-link>
						<router-link to="#3">IT·프로그래밍</router-link>
						<router-link to="#4">영상·사진·음향</router-link>
						<router-link to="#5">마케팅</router-link>
						<router-link to="#6">번역·통역</router-link>
						<router-link to="#7">문서·글쓰기</router-link>
						<router-link to="#8">비즈니스컨설팅</router-link>
						<router-link to="#9">주문제작</router-link>
						<router-link to="#10">세무·법무·노무</router-link>
					</div>
				</div>
			</section>
		</div>
	</header>
</template>

<script>
export default {
	data() {
		return {
			input_search: '',
		}
	},
	components: {},
}
</script>

<style scoped>
* {
	box-sizing: border-box;
}

#header {
	border-bottom: 1px solid #e5e5e5;
	overflow: hidden;
	/* margin-bottom: 50px; */
}
#header .sec1 {
	height: 80px;
	flex-direction: row;
	-webkit-box-align: center;
	align-items: center;
	width: 100%;
	/* margin: 0 auto; */
	/* padding: 0 16px; */
}
#header .sec2 {
	display: block;
}

#header .logo-wrap {
	width: 100px;
	display: block;
	float: left;
	margin: 20px 0;
}

#header .logo-wrap img {
	width: 100%;
}

#header #nav {
	float: right;
	display: block;
	margin-top: 20px;
	/* margin-right: 20px; */
}

#header #nav a {
	font-weight: bold;
	color: #2c3e50;
	margin-right: 20px;
}
#header #nav a:hover {
	color: #ffd500b2;
}
#header #nav a.router-link-exact-active {
	color: #ffd400;
}
/* #header .nav2 {
	text-align: center;
} */
#header .menu-wrap {
	color: grey;
	display: inline-block;
	-webkit-box-align: center;
	/* align-items: center; */
	height: 30px;
}
#header .menu-wrap a {
	float: left;
	position: relative;
	margin: 5px 10px;
	color: #222;
	font-weight: bold;
}
#header .menu-wrap > a:hover {
	border-bottom: 3px solid yellow;
}
</style>
