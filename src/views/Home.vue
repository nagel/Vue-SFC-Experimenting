<template>

  <bootstrap-card title="testing props"></bootstrap-card>

</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

// Import component from components folder
import BootstrapCard from "@/components/BootstrapCard.vue";

export default {
  name: "home",

  // Include compenent in components object
  components: {
    HelloWorld,
    BootstrapCard
  }
};
</script>
