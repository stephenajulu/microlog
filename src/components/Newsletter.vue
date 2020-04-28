<template>
  <div>
    <h4>Subscribe to my Newsletter</h4>
    <p
      class="text"
    >Don't miss out on new micro articles from me. Get notified when a new article is published.</p>
    <form
      class="form"
      method="post"
      data-netlify="true"
      onsubmit="function show_alert() { alert("Thank You For Subscribing to Ajulu s Microblog"); }"
    >
      <input
        type="text"
        name="email"
        class="form__email"
        id="email"
        onfocus="this.value=''"
        aria-label="email"
        placeholder="Email address"
      >
      <input type="hidden" value="1" name="embed">
      <input class="form__submit" type="submit" value="Subscribe">
    </form>
  </div>
</template>

<style lang="scss">
h4 {
  text-align: center;
}

.text {
  font-style: italic;
  font-size: 16px;
  text-align: center;
}

.form {
  text-align: center;
  &__email {
    padding: 13px;
    width: 15rem;
    border: 1px solid #f0f0f5;
    margin-right: 13px;
  }
  &__submit {
    border: 1px solid;
    padding: 10px;
    outline: none;
    border-radius: 2px;
    background: #fff;
    cursor: pointer;
  }
}

@media only screen and (max-width: 650px) {
  .form {
    &__submit {
      background: #fff;
      margin-top: 10px;
    }
  }
}
</style>

