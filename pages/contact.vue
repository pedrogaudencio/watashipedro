<template>
  <div class="content">
    <article class="center">
      <section>
      <input type="hidden" name="contact" netlify-honeypot="bot-field" value="contact" />
      <form name="contact" action="/thank-you" method="post" netlify>
        <label class="form-label" for="name">
          Name:
        </label>
        <input class="form-field" name="name" id="name" />
        <label class="form-label" for="email">
          Email:
        </label>
        <input class="form-field" name="email" id="email" />
        <label class="form-label" for="message">
          Message:
        </label>
        <textarea class="form-field" name="message" id="message"></textarea>
        <input class="form-button" type="submit" value="Send message" />
        <p class="hidden"><label>Don’t fill this out: <input name="bot-field"></label></p>
      </form>
      </section>
    </article>
  </div>
</template>

<script>

</script>

<style>
.hidden {
  display: none;
}
</style>
