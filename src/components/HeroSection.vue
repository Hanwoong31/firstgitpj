<template>
  <section class="hero">
    <div class="content">
      <h1 class="title">나는 음악처럼 살아간다.</h1>
      <p class="subtitle">
        감정과 이성의 균형 위에서, 창조와 해석 사이를 오가는 삶.<br />
        광고 기획자이자 카피라이터, 수학 강사였고<br />
        지금은 음악과 철학을 잇는 창작자입니다.
      </p>
      <a href="#career" class="cta-button">내 이야기 더 보기 ↓</a>
    </div>
  </section>
</template>

<script setup>
// 스크립트는 현재 필요 없음
</script>

<style scoped>
.hero {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  text-align: center;
  background: linear-gradient(135deg, #f5f7fa, #c3cfe2);
  padding: 2rem;
}

.content {
  max-width: 800px;
}

.title {
  font-size: 3rem;
  font-weight: bold;
  margin-bottom: 1.2rem;
}

.subtitle {
  font-size: 1.25rem;
  line-height: 1.8;
  color: #444;
  margin-bottom: 2rem;
}

.cta-button {
  display: inline-block;
  padding: 0.8rem 1.5rem;
  font-size: 1rem;
  background-color: #4f46e5;
  color: #fff;
  border-radius: 0.5rem;
  text-decoration: none;
  transition: background-color 0.3s ease;
}

.cta-button:hover {
  background-color: #3730a3;
}
</style>
