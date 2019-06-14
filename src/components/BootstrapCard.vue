<template>
  <div>
    <!-- Must be wrapped in a root element to display HTML -->
    <div class="card" style="width: 18rem;">
      <div class="card-body">
        <h5 class="card-title">{{ thecardtitle }}</h5>
        <p class="card-text">{{ thecardbody }}</p>
        <p class="card-text">{{ title }}</p>
        <a href="#" class="btn btn-primary">Click Here</a>
        <button @click="setTitle" class="btn btn-primary">Set Title</button>
      </div>
    </div>
  </div>
</template>

<script>
// Before using you must import the component to the view. See Home.vue.

// Must export an object for components to work
export default {
  props: ["title"],


  // Data must be a function that returns an object in a component. This is so that if a component is used multiple times on a page, their states' are independent from another.
  data() {
    return {
      thecardtitle: "The Card Title is really cool",
      thecardbody:
        "Here we have some text. It is great text, that I can tell you."
    };
  },

  methods: {
    setTitle() {
      this.thecardtitle = "Looks like you changed the title there, guy.";
    }
  }
};
</script>
