<template>
    <select @change="onSelect">
      <option value="">Select Branch</option>
      <option value="branch1">Inasal</option>
      <option value="branch2">Karenderia</option>
    </select>
  </template>
  
<script>
export default {
  methods: {
    onSelect(event) {
      const Branches = event.target.value;
      if (Branches === "branch1") {
        window.location.href = "/admin";
      } else if (Branches === "branch2") {
        window.location.href = "/menu";
      }
    },
  },
};
</script>

<style>

select {
  background-color: #fff;
  border: none;
  color: #333;
  font-size: 16px;
  padding: 8px;
}

</style>