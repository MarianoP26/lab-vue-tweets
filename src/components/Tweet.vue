<script setup>
import Actions from './Actions.vue';
import Message from './Message.vue';
import User from './User.vue';
import Timestamp from './Timestamp.vue';
import ProfileImage from './ProfileImage.vue';

defineProps({
  tweet: {
    type: Object,
    required: true,
  }
});

</script>

<template>
  <div className="tweet">
    <ProfileImage :image="tweet.user.image" />

    <div className="body">
      <div className="top">
        <User :name="tweet.user.name" :handle="tweet.user.handle"/>
        <Timestamp :time="tweet.timestamp" />
      </div>

      <Message :message="tweet.message" />
      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
