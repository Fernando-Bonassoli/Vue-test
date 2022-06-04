<template>
  <div class="home" >
    <FormSteps msg="Sobre o profissional" ></FormSteps>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import FormSteps from "@/components/FormSteps.vue";

export default {
  name: "HomeView",
  components: {
    FormSteps,
  },
};
</script>
