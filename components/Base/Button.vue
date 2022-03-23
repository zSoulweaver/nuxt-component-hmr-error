<template>
  <button class="b-button" :class="{ 'b-button--disabled': disabled }">
    <slot />
  </button>
</template>

<script setup>
defineProps({
  disabled: Boolean
})
</script>

<style>
.b-button {
  background-color: rebeccapurple;
  padding: 1rem;
  border-radius: 0.5rem;
  color: #fff;
  font-weight: 600;
}

.b-button--disabled {
  opacity: 0.5;
}
</style>