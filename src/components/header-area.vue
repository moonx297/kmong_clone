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
					<router-link to="/cate-design">디자인</router-link>
					<router-link to="#">전문가 등록</router-link>
					<router-link to="#1">로그인</router-link>
					<router-link to="#2">무료 회원가입</router-link>
				</nav>
			</section>

			<section class="sec2">
				<div class="nav2">
					<div class="menu-wrap">
						<li><a href="#">디자인</a></li>
						<li><a href="#">IT·프로그래밍</a></li>
						<li><a href="#">영상·사진·음향</a></li>
						<li><a href="#">마케팅</a></li>
						<li><a href="#">번역·통역</a></li>
						<li><a href="#">문서·글쓰기</a></li>
						<li><a href="#">비즈니스컨설팅</a></li>
						<li><a href="#">주문제작</a></li>
						<li><a href="#">세무·법무·노무</a></li>
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
section {
	display: block;
}
#header .sec1 {
	height: 74px;
	flex-direction: row;
	-webkit-box-align: center;
	align-items: center;
	width: 100%;
	margin: 0 auto;
	/*padding: 0 16px;*/
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
	margin-right: 20px;
}

#header #nav a {
	font-weight: bold;
	color: #2c3e50;
	margin-right: 20px;
}

#header #nav a.router-link-exact-active {
	color: #ffd400;
}
#header .nav2 {
	display: inline-block;
}
#header .menu-wrap {
	color: grey;
	display: inline-block;
	-webkit-box-align: center;
	align-items: center;
	height: 30px;
	text-align: center;
}
#header .menu-wrap li {
	float: left;
	position: relative;
	margin: 5px 10px;
}

#header .menu-wrap li a {
	display: block;
}

#header .menu-wrap li:hover > a {
	font-weight: bold;
	border-bottom: 3px solid yellow;
	overflow: visible;
}

#header .menu-wrap ul li {
	float: none;
}
#header .menu-wrap ul li:hover a {
	font-weight: bold;
}
#header .menu-wrap ul {
	position: absolute;
	text-align: center;
	opacity: 0;
}
#header .menu-wrap li:hover ul {
	opacity: 1;
}
#header .menu-wrap li:hover ul li {
	height: 35px;
	overflow: visible;
}
</style>
