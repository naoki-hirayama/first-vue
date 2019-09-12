<template>
  <div>
    <slot name="title" v-bind:user="user" text="text"></slot>
    <slot></slot>
    <hr>
    <P>いいねの数</P>
    <slot name="number"></slot>
  </div>
</template>

<script>
export default {
  data() {
    return {
      user: {
        firstName: "Jack",
        lastName: "Donald"
      }
    };
  }
};
</script>

<style scoped>
h1 {
  color: red;
}
</style>
