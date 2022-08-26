<template>
	<header id="header">
		<div class="container">
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
			</nav>
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
#header {
	border-bottom: 1px solid #e5e5e5;
	overflow: hidden;
	margin-bottom: 50px;
}

#header .logo-wrap {
	width: 100px;
	float: left;
	margin: 20px 0;
}

#header .logo-wrap img {
	width: 100%;
}

#header #nav {
	float: right;
	margin-top: 20px;
}

#header #nav a {
	font-weight: bold;
	color: #2c3e50;
}

#header #nav a.router-link-exact-active {
	color: #ffd400;
}
</style>
