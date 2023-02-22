<script setup>
import { defineProps } from "vue";

const { second, question } = defineProps(["second,question"]);
</script>

<template>
  <main>
    <div>
      {{ second }}
    </div>
    <div>
      {{ question }}
    </div>
  </main>
</template>
