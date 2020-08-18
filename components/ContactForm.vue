<template>
  <form action="https://formspree.io/xqkyokvp" method="POST">
    <div class="field">
      <div class="control">
        <label class="label" for="name">Your Name:</label>
        <input class="input is-info" type="text" name="name" required="true" :placeholder="namePlaceholderText">
      </div>
    </div>
    <div class="field">
      <div class="control">
        <label class="label" for="email">Your Email:</label>
        <input class="input is-info" type="email" name="email" required="true" :placeholder="emailPlaceholderText">		
      </div>			
    </div>
    <div class="field">
      <div class="control">
        <label class="label" for="message">Message:</label>
        <textarea class="textarea is-info" name="message" required="true" :placeholder="messagePlaceholderText" ></textarea>
      </div>					
    </div>
    <div class="field has-text-centered">
      <button class="button is-primary" type="submit">Send</button>
    </div>
  </form>
</template>

<script>
export default {
  data: function() {
    return {
      namePlaceholderText: "Buffy Summers",

      emailPlaceholderText: "bsummers@sunnydalehighschool.edu",

      messagePlaceholderText: "Hey Sam! Just checking in to see if you got my memo about the Hellmouth opening up nearby. Hope to hear back soon! Signed, Buffy"
    }
  }
}
</script>

<style>

</style>