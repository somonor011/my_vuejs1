
<template>
  <div>
    <button @click="chageText()">Change Text</button>
    <h1>{{ txt }}</h1>
  </div>
</template>

<script>
  
  // Option API
  export default{
    data() {
      return {
        txt : "Hello VueJS",
      }
    },
    methods: {
      chageText(){
        this.txt = "What's up VueJS ?"
      }
    },
  }

</script>