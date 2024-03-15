<template>
  <div class="card">
    <div class="card-body">
      <h1 class="card-title fw-bold">My Info</h1>
      <h2 class="card-subtitle fs-5 fw-semibold">Mobile Phone</h2>
      <p class="card-text">090-</p>
      <button class="btn btn-outline-primary btn-sm mx-1" @click="showSubj()">
        Subject
      </button>
      <div class="card-body" v-if="isShow">
        <SubjList />
      </div>
    </div>
  </div>
</template>

<script>
import SubjList from "./SubjList.vue";
export default {
  name: "InfoList",
  components: {
    SubjList,
  },
  data() {
    return {
      isShow: false,
    };
  },

  methods: {
    showSubj() {
      this.isShow = !this.isShow;
    },
  },
};
</script>

<style>
</style>