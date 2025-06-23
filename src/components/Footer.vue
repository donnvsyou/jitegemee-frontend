<template>
  <v-footer class="text-center d-flex flex-column ga-2 py-4" color=#64B5F6
>
    <div class="d-flex ga-3">
      <v-btn
        v-for="icon in icons"
        :key="icon"
        :icon="icon"
        density="comfortable"
        variant="text"
      ></v-btn>
    </div>

    <v-divider class="my-2" thickness="2" width="50"></v-divider>

    <div class="text-caption font-weight-regular opacity-60">
      At Jitegemee, we blend academic excellence with innovation and creativity. Our programs are designed to challenge, inspire, and prepare students for impactful careers and lifelong learning in a rapidly changing world.
    </div>

    <v-divider></v-divider>

    <div>
      {{ new Date().getFullYear() }} — <strong>Jitegemee</strong>
    </div>
  </v-footer>
</template>
<script setup>
  const icons = [
    'mdi-facebook',
    'mdi-twitter',
    'mdi-linkedin',
    'mdi-instagram',
  ]
</script>