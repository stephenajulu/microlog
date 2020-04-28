<template>
  <div>
  <h2 class="title">Oops, Page Not Found</h2>
    <g-link to="/" class="gohome">Go Home</g-link>
    <div class="icon">
      <g-image src="../assets/images/404.svg"></g-image>
    </div>
  </div>
</template>

<style scoped>
.icon {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.title, .gohome {
justify-content: center;
align-items: center;
text-align: center;
}
</style>
