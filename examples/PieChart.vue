<template>
  <div id="app">
    <vue-frappe
      id="test"
      title="Monthly Distribution"
      type="pie"
      :height="300"
      :labels="['Sun', 'Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']"
      :lineOptions="{regionFill: 1}"
      :colors="['red']"
      :discreteDomains="false"
      :dataSets="this.data"
    ></vue-frappe>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      data: [
        {
          values: [18, 40, 30, 35, 8, 52, 17, -4],
        },
      ],
    };
  },
};
</script>