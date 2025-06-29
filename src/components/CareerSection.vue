<template>
  <section id="career" class="career-section">
    <h2 class="section-title">나의 경력</h2>
    <div class="card-grid">
      <div class="card" v-for="(item, index) in careers" :key="index">
        <div class="icon">{{ item.icon }}</div>
        <h3 class="card-title">{{ item.title }}</h3>
        <p class="card-description">{{ item.description }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
const careers = [
  {
    title: '광고회사 기획자 & 카피라이터',
    description: '브랜드 캠페인을 기획하고 카피를 제작했습니다. 메시지와 감정을 잇는 문장을 고민했습니다.',
    icon: '📝',
  },
  {
    title: '수학 강사',
    description: '논리적 사고와 설명 능력을 기르며 수많은 학생과 함께 수학의 아름다움을 나눴습니다.',
    icon: '📐',
  },
  {
    title: '음악 창작자',
    description: '로직 프로를 활용해 음악을 만들고, 감정과 사유를 음으로 표현하고 있습니다.',
    icon: '🎵',
  },
];
</script>

<style scoped>
.career-section {
  padding: 4rem 1rem;
  background-color: #f9fafb;
  text-align: center;
}

.section-title {
  font-size: 2.2rem;
  font-weight: bold;
  margin-bottom: 2.5rem;
}

.card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
  max-width: 1000px;
  margin: 0 auto;
}

.card {
  background: white;
  border-radius: 1rem;
  padding: 2rem;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.05);
  transition: transform 0.2s ease;
}

.card:hover {
  transform: translateY(-5px);
}

.icon {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.card-title {
  font-size: 1.3rem;
  font-weight: 600;
  margin-bottom: 0.8rem;
}

.card-description {
  font-size: 1rem;
  color: #555;
  line-height: 1.6;
}
</style>
