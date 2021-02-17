<template>
  <div class="col-full">
    <h1 :class="[$style.headingLarge,$style.centered]">404 Not found</h1>
    <p :class="[$style.textLarge ,$style.centered]">Oooops, we coudn't find what you are looking for. Why don't you
      <router-link :to="{name: 'PageHome'}">go home instead?</router-link>
    </p>
  </div>
</template>

<script>
export default {
  name: 'PageNotFound'
}
</script>

<style module>
.headingLarge {
  font-size: 100px;
}

.textLarge {
  font-size: 50px;
  font-weight: 100;

}

.centered {
  text-align: center;
}
</style>
