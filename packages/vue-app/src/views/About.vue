<template>
  <div class="about">
    <h1>This is an about page</h1>
    <MyButton @click="clicked">button</MyButton>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "@vue/composition-api";
import MyButton from "@/components/MyButton.vue"; // @ is an alias to /src

export default defineComponent({
  name: "About",
  components: {
    MyButton,
  },
  setup(){
    return {
      clicked: ()=> window.alert("clicked")
    }
  }
});
</script>