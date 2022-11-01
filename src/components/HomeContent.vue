<template>
  <div class="main-content">
    <h2 class="my-5 text-center" v-if="!isAuthenticated">Not logged in</h2>
    <h2 class="my-5 text-center" v-else> Logged in</h2>

  </div>
</template>

<script>
import {useAuth0} from "@auth0/auth0-vue";

export default {
  name: "HomeContent",
  setup() {
    const auth0 = useAuth0();

    return {
      isAuthenticated: auth0.isAuthenticated,
      user: auth0.user
    }
  }
};
</script>
