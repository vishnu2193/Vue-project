<template>
  <div>
Hello child
  </div>
  <!-- Access the props -->
  <div>{{Vis}}</div>
  <div>{{Text}}</div>
</template>

<script>
export default {
  // receiving props below
  props:['Vis',"Text"],
  name: "HelloWorld",
  // props: {
  //   msg: String,
  // },
};
</script>

