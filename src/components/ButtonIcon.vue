<script setup>
</script>

<template>
  <button class="button-icon">
    <slot />
  </button>
</template>

<style lang="scss" scoped>
button {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 8px;
  background: transparent;
  margin: 4px;
  border: none;
  border-radius: 7px;
  transition: 0.2s;
  .svg-icon {
    // color: var(--color-text);
    color: black;
    height: 16px;
    width: 16px;
  }
  &:first-child {
    margin-left: 0;
  }
  &:hover {
    // background: var(--color-secondary-bg-for-transparent);
    background: rgba($color: #d0d0d0, $alpha: 1);
  }
  &:active {
    transform: scale(0.92);
    background: rgba($color: #d0d0d0, $alpha: 1);
  }
}
</style>
