<script>
import { ref } from "vue";
// import { RouterView } from "vue-router";
// // import DragableViewVue from "./components/DragableView.vue";
// import HomeView from "./components/HomeView.vue";

export default {
  setup() {
    const user = ref({
      name: "kamal",
      age: 21,
    });
    //using reactive word replace with ref to doesn't use user.value
    console.log(user);
    return { username: user.value.name, age: user.value.age, user: user };
  },
};
</script>
<template>
  <div>
    <!-- <HomeView /> -->
    <!-- <span v-text="msg"></span>

    <span>{{ msg }}</span> -->
    <h1>
      {{ username }}
    </h1>
    <h1>
      {{ user }}
    </h1>
    <!-- {{ value }} -->
  </div>
</template>
