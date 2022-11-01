<template>
  <div>
    <home-content />
  </div>
</template>

<script>
import HomeContent from "../components/HomeContent";

export default {
  name: "home",
  components: {
    HomeContent,
  },
};
</script>

<style lang="css" scoped>
.main-content .fa-link {
    margin-right: 5px;
}
</style>
