<template>
  <img
      :src="profileImage"
      className="profile"
      alt="profile"
    />
</template>

<script>
export default {
    name: "ProfileImage",
    props: {
        profileImage: {
            type: String,
        },
    },
}
</script>

<style>

</style>