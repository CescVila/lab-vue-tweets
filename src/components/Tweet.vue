<template>
  <div className="tweet">
    <ProfileImage  :profileImage="tweet.user.image"/>

    <div className="body">
      <div className="top">
        <UserComponent :userComponent="tweet.user"/>
        <TimesTamp :timesTamp="tweet.timesTamp"/>
      </div>

      <MessageComponent :message="tweet.message"/>

      <ActionsComponent />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>
<script>
import UserComponent from "./UserComponent.vue";
import TimesTamp from "./TimesTamp.vue";
import ProfileImage from "./ProfileImage.vue";
import MessageComponent from "./MessageComponent.vue";
import ActionsComponent from "./ActionsComponent.vue";

export default {
  name: "Tweet",
  components: {
    UserComponent,
    TimesTamp,
    ProfileImage,
    MessageComponent,
    ActionsComponent,
  },
  props:{
    tweet: Object,
  }
}
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
