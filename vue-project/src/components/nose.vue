<template></template>
<h1>loko {{firstName}} + {{lastName}}</h1>
<script>
import ref, { watch } from "vue";

// const firstName = ref("John");
// const lastName = ref("Doe");

// const loko = () => {
//   return firstName + " " + lastName;
// };

let volume = ref(0);

watch(volume, (newValue, oldValue) => {
  if (newValue === 8) {
  }
});

const movieList = ref(["Bataman", "Spiderman"]);

function addMovie() {
  movieList.value.push("Saving Private Ryan");
}

watch(
  movieList,
  (newValue, oldValue) => {
    console.log(`Updated:  ${newValue}`);
  },
//   { deep: true }
);
</script>

<style></style>
