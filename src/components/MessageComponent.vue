<template>
  <p className="message">
        {{message}}
      </p>
</template>

<script>
export default {
    name: "MessageComponent",
    props: {
      message: String,
    },

};
</script>

<style>

</style>