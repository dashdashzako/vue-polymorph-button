<template>
  <component
    :is="$attrs.href ? 'a' : 'button'"
    v-bind="$attrs"
    class="base-button"
    ><slot>Default text</slot></component
  >
</template>

<style scoped>
.base-button {
  display: inline-block;
  padding: 0.25rem 0.5rem;

  color: #333;
  cursor: pointer;
  border: 2px solid #333;
  background-color: #efefe5;
  border-radius: 4px;

  text-decoration: none;
  font-size: 100%;
  font-family: inherit;
  line-height: 1;
}
</style>
