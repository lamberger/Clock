<template>
    <div>
        <h1>{{ currentTime }}</h1>
        <h2>{{ time }}</h2>
    </div>
</template>

<script>
import moment from "moment";
export default {
  data() {
    return {
      time: null,
      currentTime: "Current time"
    };
  },
  methods: {
    display() {
      this.time = moment().format("HH:mm:ss");
    }
  },
  //Called synchronously after the instance is created.
  created() {
    this.time = moment().format("HH:mm:ss");
    setInterval(() => this.display(), 1000);
  }
}
</script>
