<template>
    <body>
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
            <a class="navbar-item">
              About Me
            </a>
            <a class="navbar-item">
              Projects
            </a>
            <a class="navbar-item">
              Contact
            </a>
          </div>
        </div>
      </nav>
      <section class="hero is-primary is-medium">
        <div class="hero-body">
          <div class="container is-centered">
            <h1 class="title is-1">
              SAM MCCALL
            </h1>
            <h2 class="subtitle is-3">
              { subtitle }
            </h2>
          </div>
        </div>
      </section>
    </body>
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
