<template>
          <span className="user">
          <span className="name">{{userComponent.name}}</span>
          <span className="handle">@{{userComponent.handle}}</span>
        </span>

</template>

<script>
export default {
    name: "UserComponent",
    props:{
        userComponent : Object,
    },
};
</script>

<style>

</style>