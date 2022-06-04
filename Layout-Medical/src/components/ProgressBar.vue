<template>
 <div class="progress mb-3" style="height: 30px; width: 400px;">
  <div class="progress-bar" role="progressbar" style="width: 49%; background: #483698;" aria-valuenow="75"  aria-valuemin="0" aria-valuemax="100">1 de 2</div>
</div>
</template>

<script>
export default {
  name: "ProgressBar",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

