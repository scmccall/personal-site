<template>
  <div class="card">
    <div class="card-image">
      <figure class="image is-128-128">
        <img src="../assets/squareimage.png">
        <!-- <img :src="imageSrc"> -->
      </figure>
    </div>
    <div class="card-content">
      <div class="content">
        <h1 class="title is-3">
          {{ projectTitle }}
        </h1>
        <p> {{ projectDescription }} 
        </p>
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
      :href="link.linkPath">
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
  ]
}
</script>

<style scoped>

</style>