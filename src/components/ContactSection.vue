<template>
  <section id="contact" class="contact-section">
    <h2 class="section-title">연락하기</h2>

    <p class="contact-description">
      함께 이야기하고 싶으신가요? 아래 연락처를 통해 자유롭게 연락해주세요.
    </p>

    <div class="contact-info">
      <div class="contact-item">
        <strong>📧 Email:</strong>
        <a :href="`mailto:${email}`">{{ email }}</a>
      </div>
      <div class="contact-item">
        <strong>🌐 GitHub:</strong>
        <a :href="github" target="_blank">내 GitHub</a>
      </div>
      <div class="contact-item">
        <strong>🎵 SoundCloud:</strong>
        <a :href="soundcloud" target="_blank">내 음악 들어보기</a>
      </div>
    </div>

    <form class="contact-form" @submit.prevent>
      <input type="text" placeholder="이름" required />
      <input type="email" placeholder="이메일" required />
      <textarea placeholder="메시지를 입력하세요" rows="5" required></textarea>
      <button type="submit">메시지 보내기</button>
    </form>
  </section>
</template>

<script setup>
const email = 'your.email@example.com';
const github = 'https://github.com/yourusername';
const soundcloud = 'https://soundcloud.com/yourname';
</script>

<style scoped>
.contact-section {
  padding: 4rem 1rem;
  background-color: #eef2f7;
  text-align: center;
}

.section-title {
  font-size: 2.2rem;
  font-weight: bold;
  margin-bottom: 1.5rem;
}

.contact-description {
  font-size: 1rem;
  color: #555;
  margin-bottom: 2rem;
}

.contact-info {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 0.7rem;
  margin-bottom: 2.5rem;
}

.contact-item a {
  margin-left: 0.5rem;
  color: #4f46e5;
  text-decoration: none;
}

.contact-form {
  max-width: 500px;
  margin: 0 auto;
  display: grid;
  gap: 1rem;
}

.contact-form input,
.contact-form textarea {
  padding: 0.8rem;
  border: 1px solid #ccc;
  border-radius: 0.5rem;
  font-size: 1rem;
}

.contact-form button {
  padding: 0.8rem;
  background-color: #4f46e5;
  color: white;
  border: none;
  border-radius: 0.5rem;
  font-size: 1rem;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.contact-form button:hover {
  background-color: #3730a3;
}
</style>
