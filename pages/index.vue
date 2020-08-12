<template>
    <div>
      <!-- Navigation Bar -->
      <nav class="navbar is-primary is-fixed-top">
        <div class="navbar-brand">
          <a class="navbar-item" href="/">
            <img src="../assets/testImage.jpg" width="30px">
            <p>SAM MCCALL</p>
          </a>
          <a class="navbar-burger">
            <span></span>
            <span></span>
            <span></span>
          </a>
        </div>
        <div class="navbar-menu">
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
      <!-- About Me -->
      <div class="breakpoint-max">
        <section class="section" id="about">
          <div class="has-text-centered">
            <h1 class="title is-3">
              Who Am I?
            </h1>
            <h2 class="subtitle is-5">
              I am a <strong>software developer</strong> with a degree in
              Computer Science. I like creating tools that
              <strong>solve problems</strong> of all sizes. While my langauge of
              choice is <strong>Javascript</strong>, I also have experience in
              <strong>Python</strong> and <strong>Swift</strong>, and I'm a
              quick learner when it comes to interesting languages and
              frameworks to solve whatever probelm I'm faced with.
            </h2>
          </div>
        </section>
        <section class="section">
          <div class="columns">
            <div class="column">
              <div class="card">
                <header class="card-header">
                  <p class="card-header-title">
                    Front-End Skills
                  </p>
                </header>
                <div class="card-content">
                  <div class="content">
                    <ul>
                      <li>
                        Use <strong>HTML</strong>, <strong>CSS</strong>, and
                        <strong>Javascript</strong> to create beautiful and
                        interactive web pages
                      </li>
                      <li>
                        Craft websites and applications with modern front-end
                        frameworks like <strong>Vue.js</strong> and
                        <strong>React</strong>
                      </li>
                      <li>
                        Maintain legible and functional CSS using preprocessors
                        like <strong>SASS</strong>
                      </li>
                    </ul>
                  </div>
                </div>
              </div>
              <!-- <div class="card">
                <figure class="card-image is-square">
                  <img src="../assets/testImage.jpg">
                </figure>
              </div> -->
            </div>
            <div class="column">
              <!-- <div class="card">
                <figure class="card-image is-square">
                  <img src="../assets/testImage.jpg">
                </figure>
              </div> -->
              <div class="card">
                <header class="card-header">
                  <p class="card-header-title">
                    Project Skills
                  </p>
                </header>
                <div class="card-content">
                  <div class="content">
                    <ul>
                      <li>
                        Manage version control for project repositories
                        with <strong>Git</strong> using best practices
                      </li>
                      <li>
                        Build in <strong>Test-Driven Development</strong> cycles
                        using testing frameworks like <strong>Mocha</strong> and
                        <strong>Chai</strong>
                      </li>
                      <li>

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
                    Back-End Skills
                  </p>
                </header>
                <div class="card-content">
                  <div class="content">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut quisquam doloremque quae mollitia in. Incidunt magni recusandae perferendis. Earum labore ipsum vel pariatur eveniet molestias, inventore blanditiis dicta cum deserunt?
                  </div>
                </div>       
              </div>
              <!-- <div class="card">
                <figure class="card-image is-square">
                  <img src="../assets/testImage.jpg">
                </figure>
              </div> -->
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
                v-bind="project1">
              </ProjectCard>
            </div>
            <div class="column">
              <ProjectCard
                v-bind="project1">
              </ProjectCard>
            </div>
            <div class="column">
              <ProjectCard
                v-bind="project1">
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
            <div class="columns is-vcentered">
              <div class="column is-8">
                <div class="content">
                  Come chat with me if you have a project you'd like to
                  collaborate on.
                  <ul>
                    <li><a href="mailto:smccall@smccall.com">
                      Email
                    </a></li>
                    <li><a href="http://www.linkedin.com/in/sammccall/"
                          target="_blank">
                      LinkedIn
                    </a></li>
                    <li><a href="http://www.github.com/scmccall/" target="_blank">
                      GitHub
                    </a></li>
                  </ul>
                </div>
              </div>
              <div class="column">
                <figure class="image is-128x128">
                  <img src="../assets/sunset.JPG">
                </figure>
                <div class="content">
                  <p>
                    Click above to read my resume
                  </p>
                </div>
              </div>
            </div>
          </div>
        </section>
      </div>
      <!-- Footer -->
      <footer class="footer">
        
      </footer>
    </div>
</template>

<script>
export default {
  data: function() {
    return {
      project1 : {
        id : 1,
        projectTitle : "Project 1",
        imageSrc : "../assets/squareimage.png",
        projectDescription : "Here is the project description. Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempora hic quam iure ipsa eligendi dolore asperiores architecto. Eum dolores odit ipsam sapiente consequatur illum rerum quibusdam, distinctio, sit amet dolorum.",
        tags : [

          {
            tagName: "Javascript",
            tagColor: "is-info"
          },

          {
            tagName: "Node.js",
            tagColor: "is-danger"
          },

          {
            tagName: "Vue.js",
            tagColor: "is-warning"
          }

        ],

        links : [
          {
            linkName: "Live Demo",
            linkPath: "/"
          },

          {
            linkName: "See Source",
            linkPath: "github.com"
          }

        ]
      },
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

.breakpoint-max {
  margin: auto;
  max-width: 1300px
}
</style>
