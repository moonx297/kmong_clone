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
        <router-link to="/cate-design">전문가 등록</router-link>
        <router-link to="/cate-design">로그인</router-link>
        <router-link to="/cate-design">무료 회원가입</router-link>
      </nav>

      <ul class="menu-wrap">
        <li>
          <a href="#" id="category">전체 카테고리</a>
          <ul>
            <li><a href="#">디자인</a></li>
            <li><a href="#">IT·프로그래밍</a></li>
            <li><a href="#">영상·사진·음향</a></li>
            <li><a href="#">마케팅</a></li>
            <li><a href="#">번역·통역</a></li>
            <li><a href="#">문서·글쓰기</a></li>
            <li><a href="#">비즈니스컨설팅</a></li>
            <li><a href="#">주문제작</a></li>
            <li><a href="#">세무·법무·노무</a></li>
          </ul>
        </li>
        <li>
          <a href="#">Prime</a>
          <ul>
            <li>
              <p>TOP 2% 전문가의 서비스를 만나보세요.</p>
            </li>
          </ul>
        </li>
        <li>
          <a href="#">엔터프라이즈</a>
          <ul>
            <li>
              <p>기업 외주 전용 솔루션입니다.</p>
            </li>
          </ul>
        </li>
        <li>
          <a href="#">전자책*VOD</a>
          <ul>
            <li>
              <p>세상 모든 노하우를 배우는 곳</p>
            </li>
          </ul>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      input_search: "",
    };
  },
  components: {},
};
</script>

<style scoped>
#header {
  border-bottom: 1px solid #e5e5e5;
  overflow: hidden;
  margin-bottom: 50px;
}

#header .logo-wrap {
  width: 100px;
  display: inline-block;
  float: left;
  margin: 20px 0;
}

#header .logo-wrap img {
  width: 100%;
}

#header #nav {
  float: right;
  display: inline-block;
  margin-top: 20px;
  margin-right: 20px;
}

#header #nav a {
  font-weight: bold;
  color: #2c3e50;
}

#header #nav a.router-link-exact-active {
  color: #ffd400;
}
#header .menu-wrap {
  float: bottom;
  display: block;
}
#header .menu-wrap li {
  float: left;
  position: relative;
  margin: 5px 30px;
}

#header .menu-wrap li a {
  display: block;
}

#header .menu-wrap li:hover > a {
  font-weight: bold;
  border-bottom: 3px solid yellow;
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
