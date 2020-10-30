<template>
    <div>
      <!-- Navigation Bar -->
      <nav class="navbar is-primary is-fixed-top">
        <div class="navbar-brand">
          <a class="navbar-item" href="/">
            <p>SAM MCCALL</p>
          </a>
          <a class="navbar-burger"
          :class="{ 'is-active' : navBarIsActive }"
          @click="navBarIsActive = !navBarIsActive">
            <span></span>
            <span></span>
            <span></span>
          </a>
        </div>
        <div class="navbar-menu"
        :class="{ 'is-active' : navBarIsActive }">
          <div class="navbar-end">
            <a href="/#about" class="navbar-item">
              About Me
            </a>
            <a href="/#projects" class="navbar-item">
              Projects
            </a>
            <a href="/#contact" class="navbar-item">
              Contact
            </a>
          </div>
        </div>
      </nav>
      <!-- Hero Image -->
      <section class="hero is-primary is-large">
        <div class="hero-body ">
          <div class="">
            <h1 class="title is-1">
              SAM MCCALL
            </h1>
            <h2 class="subtitle is-4">
              SOFTWARE DEVELOPER
            </h2>
          </div>
        </div>
      </section>
      <div class="max-width-container">
        <!-- About Me -->
        <section class="section" id="about">
          <div class="has-text-centered">
            <h1 class="title is-3">
              Who Am I?
            </h1>
          </div>
          <AboutMe />
        </section>
        <!-- Skills Section -->
        <section class="section">
          <div class="columns">
            <div class="column">
              <div class="card">
                <header class="card-header">
                  <p class="card-header-title">
                    Front-End
                  </p>
                </header>
                <div class="card-content">
                  <div class="content">
                    <ul>
                      <li>
                        Use <strong>HTML</strong>, <strong>CSS</strong>, and <strong>Javascript</strong> to create responsive and interactive web pages
                      </li>
                      <li>
                        Craft websites and applications with modern front-end frameworks like <strong>Vue.js</strong> and <strong>React</strong>
                      </li>
                      <li>
                        Maintain legible and functional CSS using preprocessors like <strong>SASS</strong>
                      </li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
            <div class="column">
              <div class="card">
                <header class="card-header">
                  <p class="card-header-title">
                    Back-End
                  </p>
                </header>
                <div class="card-content">
                  <div class="content">
                    <ul>
                      <li>
                        Build efficient and algorithm-driven back-end servers in Javascript using <strong>Node.js</strong>
                      </li>
                      <li>
                        Make RESTful API calls using <strong>axios</strong>, <strong>mongoose</strong>, and <strong>express</strong> to manipulate JSON data
                      </li>
                      <li>
                        Connect applications to back-end databases using <strong>MongoDB</strong>
                      </li>
                    </ul>
                  </div>
                </div>       
              </div>
            </div>
            <div class="column">
              <div class="card">
                <header class="card-header">
                  <p class="card-header-title">
                    Project Management
                  </p>
                </header>
                <div class="card-content">
                  <div class="content">
                    <ul>
                      <li>
                        Manage version control for project repositories with <strong>Git</strong> using best practices
                      </li>
                      <li>
                        Implement <strong>unit tests</strong> using testing frameworks like <strong>Mocha</strong> and <strong>Chai</strong>
                      </li>
                      <li>
                        Stay connected with both remote and onsite staff with <strong>Slack</strong>, <strong>Skype</strong>, and <strong>Zoom</strong>
                      </li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>
        <!-- Portfilio Projects -->
        <section class="section" id="projects">
          <h1 class="title is-2 has-text-centered">
            Projects
          </h1>
          <div class="columns">
            <div class="column">
              <ProjectCard
                v-bind="projectsList.projects[0]">
              </ProjectCard>
            </div>
            <div class="column">
              <ProjectCard
                v-bind="projectsList.projects[1]">
              </ProjectCard>
            </div>
            <div class="column">
              <ProjectCard
                v-bind="projectsList.projects[2]">
              </ProjectCard>
            </div>
          </div>
        </section>
        <!-- Contact -->
        <section class="section" id="contact">
          <h1 class="title is-2 has-text-centered">
            Get in touch
          </h1>
          <div class="box">
            <div class="contact-width-container">
              <ContactForm />
            </div>
          </div>
        </section>
      </div>
      <!-- Footer -->
      <footer class="footer">
        <div class="has-text-centered">
          <div class="content">
            © 2020 — Designed and coded by Sam McCall using
            <a href="https://vuejs.org/">Vue.js</a> + 
            <a href="https://nuxtjs.org/">Nuxt</a> + 
            <a href="https://bulma.io">Bulma</a>.
          </div>
        </div>
      </footer>
    </div>
</template>

<script>

import projectJSON from "../assets/projectJSON.json"

export default {
  metaInfo: {
    title: "Sam McCall",
    titleTemplate: null,
  },
  data: function() {
    return {

      projectsList : projectJSON,

      navBarIsActive: false,

    }
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

.max-width-container {
  margin: auto;
  max-width: 1240px
}

.contact-width-container {
  margin: auto;
  max-width: 600px
}

.navbar-menu {
  margin-right: 20px;
}
</style>
