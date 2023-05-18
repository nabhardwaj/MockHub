<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
    <div class="greetings">
      <h3>
        <a href="" target="" rel="noopener">Login</a> +
        <a href="" target="" rel="noopener">Register</a>
        <span class="green">{{ msg }}</span>
      </h3>
    </div>
</template>

<style scoped>

</style>