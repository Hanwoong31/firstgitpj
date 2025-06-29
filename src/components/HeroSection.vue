<template>
  <section class="hero">
    <!-- 배경 이미지 오버레이 -->
    <div class="overlay"></div>

    <!-- 실제 내용 -->
    <div class="content">
      <h1 class="title">나는 음악처럼 살아간다.</h1>
      <p class="subtitle">
        감정과 이성의 균형 위에서,<br />
        창조와 해석 사이를 오가는 삶.<br />
        광고 기획자이자 카피라이터, 수학 강사였고,<br />
        지금은 음악과 철학을 잇는 창작자입니다.
      </p>
      <a href="#career" class="cta-button">내 이야기 더 보기 ↓</a>
    </div>
  </section>
</template>

<script setup>
// 특별한 로직 없음
</script>

<style scoped>
.hero {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  padding: 2rem;
  text-align: center;
  background: linear-gradient(135deg, #4e2a1e, #8b3a2c); /* 바이올린 느낌 */
  background-size: cover;
  background-position: center;
  overflow: hidden;
}

/* 이미지 오버레이 */
.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: url('/01_sunrise.png'); /* public 폴더의 이미지 사용 */
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  opacity: 0.15; /* 은은하게 */
  z-index: 1;
}

/* 콘텐츠는 위에 떠있게 */
.content {
  position: relative;
  z-index: 2;
  max-width: 800px;
}

/* 타이틀 텍스트 */
.title {
  font-size: 3rem;
  font-weight: bold;
  margin-bottom: 1.2rem;
  color: #ffffff;
}

/* 서브텍스트 */
.subtitle {
  font-size: 1.25rem;
  line-height: 1.8;
  color: #e0e0e0;
  margin-bottom: 2rem;
}

/* CTA 버튼 */
.cta-button {
  display: inline-block;
  padding: 0.8rem 1.5rem;
  font-size: 1rem;
  background-color: #ffffffcc;
  color: #4e2a1e;
  border-radius: 0.5rem;
  text-decoration: none;
  transition: background-color 0.3s ease;
}

.cta-button:hover {
  background-color: #fff;
}
</style>
