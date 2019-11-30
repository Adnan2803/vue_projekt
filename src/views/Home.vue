<template>
  <div class="home">
    <div class="container">
      <div class="row">
        <div class="col-md-1"></div>
        <div class="col-md-7">
          <InstaCard />
        </div>
        <div class="col-md-4"></div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import InstaCard from "@/components/InstaCard.vue";

export default {
  name: "home",
  components: {
    InstaCard
  }
};
</script>
