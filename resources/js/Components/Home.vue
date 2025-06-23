<template>
  <div class="home-container">
    <h1> Hello, I'm Harsh Raj Singh</h1>
    <p class="intro">
      Welcome to my portfolio web app! I’m a passionate Data Scientist and Developer with a strong background in AI and web technologies. This app showcases my skills, experience, and projects, built using modern tools.
    </p>

    <section class="tech-highlight">
      <h2>About this Web Application</h2>
      <p>
        This app is built with <strong>Laravel</strong> for backend routing, <strong>Vue.js</strong> for a dynamic frontend, and <strong>Inertia.js</strong> to create a seamless single-page application experience without a full SPA framework complexity.
      </p>
    </section>

    <section class="call-to-action">
      <p>
        Feel free to explore my <router-link to="/about">About Me</router-link> page to learn more about my background, skills, and why I’m excited about opportunities at companies like Teemill.
      </p>
    </section>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>

<style scoped>
.home-container {
  max-width: 700px;
  margin: 3rem auto;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #333;
  padding: 1rem;
  text-align: center;
}

h1 {
  font-size: 2.4rem;
  color: #42b883;
  margin-bottom: 1rem;
}

.intro {
  font-size: 1.3rem;
  line-height: 1.5;
  margin-bottom: 2rem;
}

.tech-highlight {
  background-color: #e6f3ec;
  border-left: 6px solid #42b883;
  padding: 1rem 1.5rem;
  margin-bottom: 2rem;
  border-radius: 8px;
  font-style: italic;
  font-size: 1.1rem;
  color: #2f5d38;
}

.call-to-action p {
  font-weight: 600;
  font-size: 1.1rem;
}

router-link {
  color: #42b883;
  text-decoration: none;
  font-weight: bold;
}

router-link:hover {
  text-decoration: underline;
}
</style>
