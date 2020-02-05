<template>
  <div>
    <h2>Left Nav Component</h2>
    <div>Age is : {{age}}</div>
    <button @click="IncrementAge()">Increment Age</button>
  </div>
</template>
<script>
export default {
  props: {
    age: Number,
    IncrementAge: Function
  }
};
</script>
