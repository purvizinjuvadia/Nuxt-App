<template>
  <section class="post-list">
    <PostPreview
      id="1"
      :is-admin="isAdmin"
      thumbnail="https://codingthesmartway.com/wp-content/uploads/2017/01/02.png"
      title="Hello there!"
      previewText="This is my first post">
    </PostPreview>
    <PostPreview
      id="2"
      :is-admin="isAdmin"
      thumbnail="https://codingthesmartway.com/wp-content/uploads/2017/01/02.png"
      title="Hello there - the second time!"
      previewText="This is my second post">
    </PostPreview>
    <PostPreview
      id="3"
      :is-admin= "isAdmin"
      thumbnail="https://codingthesmartway.com/wp-content/uploads/2017/01/02.png"
      title="Hello there - the third time!"
      previewText="This is my third post">
    </PostPreview>
  </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'
export default {
  components: {
    PostPreview
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false
    }
  }
}
</script>

<style>
  .post-list {
    display: flex;
    padding: 20px;
    box-sizing: border-box;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
  }

</style>
