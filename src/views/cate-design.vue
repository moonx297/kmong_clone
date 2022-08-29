<template>
	<div class="container">
		<div class="image1-text">
			<img src="@/assets/images/head banner.png" />
		</div>
		<aside id="aside">
			<h2>디자인</h2>
			<div class="image-text">
				<img src="@/assets/images/aside banner.webp" />
			</div>
			<ul>
				<li>
					<a href="#">로고·브랜딩</a>
				</li>
				<li>
					<a href="#">상세·이벤트 페이지</a>
				</li>
				<li>
					<a href="#">명함·인쇄·홍보물</a>
				</li>
				<li>
					<a href="#">PPT·인포그래픽</a>
				</li>
				<li>
					<a href="#">웹·모바일</a>
				</li>
				<li>
					<a href="#">패키지 디자인</a>
				</li>
				<li>
					<a href="#">일러스트·캐리커쳐</a>
				</li>
				<li>
					<a href="#">웹툰·캐릭터·이모티콘</a>
				</li>
				<li>
					<a href="#">블로그·SNS·썸네일</a>
				</li>
				<li>
					<a href="#">포토샵·파일변환</a>
				</li>
				<li>
					<a href="#">제품·3D프린팅</a>
				</li>
				<li>
					<a href="#">공간디자인</a>
				</li>
				<li>
					<a href="#">북·앨범디자인</a>
				</li>
				<li>
					<a href="#">캘리그라피·폰트</a>
				</li>
				<li>
					<a href="#">메타버스·NFT아트</a>
				</li>
				<li>
					<a href="#">VR·AR·게임</a>
				</li>
				<li>
					<a href="#">의류디자인</a>
				</li>
				<li>
					<a href="#">간판·시공</a>
				</li>
				<li>
					<a href="#">템플릿</a>
				</li>
				<li>
					<a href="#">기타</a>
				</li>
			</ul>
		</aside>
		<main id="main">
			<p class="page-navigation">홈>디자인</p>
			<table class="table-text">
				<tr>
					<td align="center" onClick="location.href='#'">주말 작업 여부</td>
					<td onClick="location.href='#'">주말 상담 가능</td>
					<td onClick="location.href='#'">주말 작업 가능</td>
					<td onClick="location.href='#'">주말 불가능</td>
				</tr>
			</table>
			<ContentArea />
		</main>
	</div>
</template>

<script>
import ContentArea from '@/components/content-area.vue'
export default { components: { ContentArea } }
</script>

<style scoped>
#aside {
	float: left;
	width: 15%;
	box-sizing: border-box;
	height: 100%;
	margin-right: 5%;
	text-align: left;
	/* padding: 30px 0; */
}

#aside h2 {
	padding: 15px 0;
	margin-bottom: 17px;
	border-bottom: 2px solid #ffdd00;
}

#aside li {
	margin-bottom: 15px;
}

#main {
	width: 80%;
	padding: 18px 0;
	float: right;
}

#main .page-navigation {
	margin-bottom: 10px;
}

#main table td:first-child {
	background: #f9f9f9;
	border-right: 1px solid #e5e5e5;
}
.table-text {
	margin-bottom: 30px;
}
.image-text {
	margin-bottom: 20px;
}
.image-text img {
	width: 100%;
}
.image1-text img {
	width: 100%;
}
</style>
