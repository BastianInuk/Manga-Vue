<template>
  <div class="about">
    <AboutPage msg='About Manga DK'/>
  </div>
</template>

<script lang="ts">
import AboutPage from '@/components/AboutPage.vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'About',
  components: {
    AboutPage,
  },
});
</script>
