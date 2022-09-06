<template>
  <div :class="backgroundColor">
    <div v-if="showString">
      {{ printString() }}
    </div>

    <button @click="changeBackground()">Change the background color</button>
  </div>
</template>
    
    <script>
export default {
  data() {
    return {
      name: "Pepe",
      showString: true,
      posts: [
        {
          title: "How to makeup",
          content: "How to makeup a woman",
          description: "test",
        },
        {
          title: "How to makeup2",
          content: "How to makeup a woman2",
          description: "test2",
        },

        {
          title: "How to makeup3",
          content: "How to makeup a woman3",
          description: "test3",
        },
      ],
      backgroundColor: "",
    };
  },
  methods: {
    printString() {
      return "Hello";
    },
    changeBackground() {
      this.backgroundColor = "footer";
    },
  },
  created() {
    //console.log("hello");
  },
};
</script>
    
<style scoped>
.footer {
  background-color: rebeccapurple;
}
</style>