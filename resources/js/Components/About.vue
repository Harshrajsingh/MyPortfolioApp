<template>
  <div class="about-container">
    <h1>About Me</h1>

    <div class="profile">
      <img src="/images/harsh-profile.jpg" alt="Harsh Raj Singh" class="profile-img" />
      <div class="summary">
        <p>
          I'm Harsh Raj Singh, a dedicated developer and data scientist with a Master's in Data Science with AI, and ~3 years of industry experience. I’m passionate about building smart, scalable web apps and working with cutting-edge technologies.
        </p>
      </div>
    </div>

    <section class="why-teemill">
      <h2>Why I am interested in Teemill</h2>
      <p>
        I admire Teemill's commitment to sustainability and innovation in the e-commerce space. Your focus on creating environmentally-friendly, scalable platforms resonates with my passion for technology that drives positive impact. I’m excited about contributing my skills in Laravel and Vue.js to build performant, user-friendly applications that align with Teemill’s mission.
      </p>
    </section>

    <section class="experience">
      <h2>Experience & Education</h2>
      <ul>
        <li><strong>AI Trainer/Coder (Freelance)</strong> - Outlier AI, London (Jan 2025 - Present)</li>
        <li><strong>AI/ML Intern</strong> - Nethermind, London (Oct 2024 - Jan 2025)</li>
        <li><strong>System Engineer</strong> - Tata Consultancy Services (Enbridge Gas), India (Feb 2021 - Sept 2023)</li>
        <li><strong>Data Science & ML Intern</strong> - Code Bucket, India (May 2019 - July 2019)</li>
        <li><strong>MSc Data Science with AI, 1st Class Honours</strong> - Bournemouth University (2023 – 2024)</li>
        <li><strong>BTech Computer Science</strong> - CUSAT (2016 - 2020)</li>
      </ul>
    </section>

    <section class="skills-section">
      <h2>Skills & Technical Expertise</h2>
      <div v-for="skill in skills" :key="skill.name" class="skill-bar">
        <span>{{ skill.name }}</span>
        <div class="bar-bg">
          <div class="bar-fill" :style="{ width: skill.level + '%' }"></div>
        </div>
      </div>

      <h3 class="mt-3">Tools and Languages:</h3>
      <ul>
        <li>Git, Docker, Jupyter Notebook, Power BI</li>
        <li>Python, Java, SQL</li>
        <li>Machine Learning, Data Science, LLM, Flask, DAX</li>
      </ul>

      <h3 class="mt-3">Technologies used to build this app:</h3>
      <ul>
        <li>Laravel (PHP framework)</li>
        <li>Vue.js (JavaScript frontend framework)</li>
        <li>Vite (modern build tool)</li>
        <li>Inertia.js (for SPA-like Laravel-Vue integration)</li>
      </ul>
    </section>

    <section class="contact">
      <h2>Contact Me</h2>
      <p>Email: <a href="mailto:harshsinghraj189@gmail.com">harshsinghraj189@gmail.com</a></p>
      <p>Mobile: +44 7552 038684</p>
      <p>LinkedIn: <a href="https://www.linkedin.com/in/harsh-s11" target="_blank">linkedin.com/in/harsh-s11</a></p>
      <p>Location: Bournemouth, UK</p>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      skills: [
        { name: 'Laravel', level: 75 },
        { name: 'Vue.js', level: 75 },
        { name: 'JavaScript', level: 75 },
        { name: 'Python', level: 90 },
        { name: 'Machine Learning', level: 90 },
      ],
    };
  },
};
</script>

<style scoped>
.about-container {
  max-width: 800px;
  margin: 2rem auto;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #444;
  padding: 1rem;
}

.profile {
  display: flex;
  align-items: center;
  gap: 1.5rem;
  margin-bottom: 2rem;
}

.profile img {
  width: 120px;
  height: 120px;
  object-fit: cover;
  border-radius: 50%;
  box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1);
}

.summary p {
  font-size: 1.2rem;
  line-height: 1.5;
}

h2 {
  margin-top: 2rem;
  margin-bottom: 1rem;
  color: #42b883;
}

h3 {
  margin-top: 1.5rem;
  margin-bottom: 0.8rem;
  color: #369a68;
}

ul {
  padding-left: 1.5rem;
  margin-bottom: 1rem;
  font-weight: 600;
}

li {
  margin-bottom: 0.5rem;
}

.why-teemill p {
  font-style: italic;
  font-size: 1.1rem;
  background-color: #e6f3ec;
  padding: 1rem;
  border-radius: 8px;
  border-left: 6px solid #42b883;
}

.skills-section .skill-bar {
  margin-bottom: 1rem;
}

.skill-bar span {
  display: inline-block;
  width: 150px;
  font-weight: 600;
}

.bar-bg {
  display: inline-block;
  width: 60%;
  height: 15px;
  background-color: #eee;
  border-radius: 8px;
  vertical-align: middle;
  overflow: hidden;
}

.bar-fill {
  height: 100%;
  background-color: #42b883;
  border-radius: 8px;
  transition: width 1.2s ease-in-out;
}

.contact p {
  margin: 0.3rem 0;
}

.contact a {
  color: #42b883;
  text-decoration: none;
  font-weight: 600;
}

.contact a:hover {
  text-decoration: underline;
}
</style>
