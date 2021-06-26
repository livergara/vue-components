<template>
  <div style="padding: 30px">
    <TagInput v-model="tags" />
    <br /><br />

    <!--Ucomment to see with features not in blog post -->
    <!-- <TagInput
      v-model="tags2"
      :options="['Hello', 'World']"
      :allowCustom="false"
      :showCount="true"
    /> -->

    <!--Ucomment to see tags synced with component -->
    <!-- <ul>
      <li v-for="tag in tags" :key="tag">{{ tag }}</li>
    </ul> -->
  </div>
</template>

<script>
import TagInput from "../components/InputTag.vue";
export default {
  name: "App",
  components: {
    TagInput: TagInput,
  },
  data() {
    return {
      tags: ["Hello", "World"],
      tags2: ["Hello"],
    };
  },
};
</script>
<style>
* {
  box-sizing: border-box;
}
</style>