<template>
  <div class="section">
    <div class="columns is-3-desktop is-8-widescreen is-1-fullhd">
      <div class="column">
        <!-- <img src="../assets/my-face.jpg"> -->
        <img src="~assets/my-face.jpg">
      </div>
      <div class="column">
        <h2 class="subtitle is-5">
          <span v-html="description"></span>
        </h2>
        <div class="level contact-link">
          <img class="level-item image is-24x24 mr-4" src="~assets/envelope.svg">
          <a class="level-item" href="mailto:smccall@smccall.com">
            smccall@smccall.com
          </a>
        </div>
        <div class="level contact-link">
          <img class="level-item image is-24x24 mr-4" src="~assets/linkedin.svg">
          <a class="level-item"
            href="http://www.linkedin.com/in/sammccall/"
            target="_blank">
            linkedin.com/in/sammccall
          </a>
        </div>
        <div class="level contact-link">
          <img class="level-item image is-24x24 mr-4"
            src="~assets/github-square.svg">
          <a class="level-item"
            href="http://www.github.com/scmccall/"
            target="_blank">
            github.com/scmccall/
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      description:
        "I’m <strong>Sam McCall</strong>, a <strong>software developer</strong> with a degree in <strong>Computer Science and Mathematics</strong>." +
        "<br><br>" +
        "I have always approached coding and development as a way of <strong>solving problems</strong>. I started coding in 2009, learning HTML on my small Netbook in order to create a custom theme for my LiveJournal page." +
        "<br><br>" + 
        "Since then I have graduated from simple HTML to a variety of tools and frameworks, but the same concept of problem solving has followed me through the years. If you take a look at my sampling of projects below, you’ll find they were all created to solve a specific problem." +
        "<br><br>" + 
        "My language of choice is <strong>Javascript</strong>. I also have experience in <strong>Python</strong> and <strong>Swift</strong>. I'm a quick learner when it comes to interesting languages and frameworks to solve whatever problem I'm faced with."

    }
  }
}
</script>

<style scoped>

.contact-link {
  float: left
}

</style>