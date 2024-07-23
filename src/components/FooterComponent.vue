<script>
export default {
  data: () => {
    return {
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-instagram',
        'mdi-youtube',
      ],
    };
  },
};
</script>

<template>
  <v-footer app class="elevation-3 text-center">
    <v-row justify="center" class="my-4 text-center">
      <v-col cols="12">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit.
        </p>
      </v-col>
      <v-col cols="12">
        <v-btn v-for="icon in icons" :key="icon" flat>
          <v-icon>{{ icon }}</v-icon>
        </v-btn>
      </v-col>
      <v-col cols="12">&copy; {{ new Date().getFullYear() }} - To Do App</v-col>
    </v-row>
  </v-footer>
</template>

<style scoped></style>
