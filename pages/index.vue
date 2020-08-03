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
            <a href="/" class="navbar-item">
              Contact
            </a>
          </div>
        </div>
      </nav>
      <!-- Hero Image -->
      <section class="hero is-primary is-fullheight-with-navbar">
        <div class="hero-body ">
          <div class="has-text-centered">
            <h1 class="title is-1">
              SAM MCCALL
            </h1>
            <h2 class="subtitle is-3">
              { subtitle }
            </h2>
          </div>
        </div>
      </section>
      <!-- About Me -->
      <section class="section" id="about">
        <div class="has-text-centered">
          <h1 class="title is-3">
            About Me
          </h1>
          <h2 class="subtitle is-5">
            Sample text sample text sample text sample text sample text 
            sample text sample text sample text sample text sample text 
            sample text sample text sample text sample text sample text 
            sample text sample text sample text sample text sample text 
          </h2>
        </div>
      </section>
      <!-- Portfilio Projects -->
      <section class="section" id="projects">
        <h1 class="title is-2 has-text-centered">
          Projects
        </h1>
        <div class="columns">
          <div class="column">
            <ProjectCard />
          </div>
          <div class="column">
            <ProjectCard />
          </div>
            <div class="column">
            <ProjectCard />
          </div>
        </div>
      </section>
      <!-- Contact -->
      <section class="section" id="contact">
        <h1 class="title is-2 has-text-centered">
          Get in touch
        </h1>
        <div class="box">
          <ul>
            <li><a href="/">
              Email
            </a></li>
            <li><a href="/">
              LinkedIn
            </a></li>
            <li><a href="/">
              GitHub
            </a></li>
          </ul>
        </div>
      </section>
      <!-- Footer -->
      <footer class="footer">
        <div class="content">
          <strong>Sam McCall</strong>
        </div>
      </footer>
    </div>
</template>

<script>
export default {}
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
</style>
