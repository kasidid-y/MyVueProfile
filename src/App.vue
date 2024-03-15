<template>
  <div class="container py-4">
    <div class="card">
      <div class="card-header">
        <div class="row row-2-col align-items-center">
          <div class="col text-center">
            <p>Kasetsart Sriracha</p>
            <h1>My Name</h1>
            <p>Some info</p>
          </div>
          <div class="col bg-info text-center">
            <img
              src="https://mdbcdn.b-cdn.net/img/Photos/new-templates/bootstrap-chat/ava1-bg.webp"
              alt="Profile"
              style="width: 150px"
              class="img-fluid"
            />
          </div>
        </div>
      </div>
      <div class="card-body">
        <InfoList />
      </div>
    </div>
  </div>
</template>

<script>
import InfoList from "./components/InfoList.vue";
export default {
  name: "App",
  components: {
    InfoList,
  },
};
</script>

<style>
</style>