<template>
  <div class="home">
    <h1> {{ title }} </h1>
    <p> {{ greeting() }} </p>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";

export default {
  data() {
    return {
      title: 'Holis Jos'
    }
  },
  methods: {
    greeting: function(){
      return 'heyyy, i didnt broke';
    }
  }
}
</script>
