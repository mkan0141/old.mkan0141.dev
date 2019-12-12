<template>
  <div class="container">
    <div class="center">
      <div class="bg-white">
        <h1 class="title text-cello font-medium text-5xl mb-10">mkan0141</h1>
        <ul class="">
          <li class="inline-block mx-8">
            <a href="https://github.com/mkan0141"><i class="fab fa-github fa-3x text-cello"></i></a>
          </li>
          <li class="inline-block mx-8">
            <a href="https://twitter.com/mkan_0141"><i class="fab fa-twitter fa-3x text-cello twitter"></i></a>
          </li>
          <li class="inline-block mx-8">
            <a href="https://speakerdeck.com/mkan0141"><i class="fab fa-speaker-deck fa-3x text-cello"></i></a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  components: {
    
  }
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  letter-spacing: 1px;
}

.title::after {
  content: "\\ｺﾝﾆﾁﾜ\/";
  font-size: 20px;
  position: absolute;
  transform: translateY(-10px) rotate(45deg);
}

.center {
  top: 50%;
}
</style>
