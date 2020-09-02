<template>
  <div class="card">
    <div class="card-image">
      <figure class="image is-4by3">
        <img :src="projectImage">
      </figure>
    </div>
    <div class="card-content">
      <div class="content">
        <h1 class="title is-3">
          {{ projectTitle }}
        </h1>
        <span v-html="projectDescription">
        </span>
      </div>
      <div class="tags">
        <span
        class="tag"
        v-for="(tag, index) in tags"
        :key="index"
        :class="tag.tagColor">
          {{ tag.tagName }}
        </span>
      </div>
    </div>
    <div class="card-footer">
      <a
      class="card-footer-item"
      v-for="(link, index) in links"
      :key="index"
      :href="link.linkPath"
      target="_blank">
        {{ link.linkName }}
      </a>
    </div>
  </div>
</template>

<script>

export default {
  props: [
    'id',
    'projectTitle',
    'imageSrc',
    'projectDescription',
    'tags',
    'links'
  ],
  computed : {
    projectImage : function () {
      if (!this.imageSrc) {
        return;
      }
      const fileName = this.imageSrc.toLowerCase()

      return require(`../assets/${this.imageSrc}`);
    }
  }
}
</script>

<style scoped>

</style>