<template>
  <div class="text-subtitle-1 ml-4">{{ date }} Uhr</div>
</template>

<script>
import { format } from "date-fns";

export default {
  data() {
    return {
      date: "",
    };
  },
  methods: {
    getDate() {
      this.date = format(new Date(), "dd.MM.yyyy, H:mm");
      setTimeout(this.getDate, 60000);
    },
  },
  mounted() {
    this.getDate();
  },
};
</script>

<style>
</style>