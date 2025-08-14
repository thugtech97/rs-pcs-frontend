<template>
  <div class="container-fluid">
    <h3 class="mb-4">Welcome User07191997</h3>

    <div class="d-flex gap-3 mb-4 flex-wrap">
      <!-- Box 1 -->
      <div class="dashboard-box flex-fill">
        <h4>Applications</h4>
        <p class="display-5">24</p>
      </div>
      <div class="dashboard-box flex-fill">
        <h4>Pending</h4>
        <p class="display-5">7</p>
      </div>
      <div class="dashboard-box flex-fill">
        <h4>Documents</h4>
        <p class="display-5">15</p>
      </div>
    </div>

    <NuxtLink class="btn btn-danger btn-md">
      Add New Application
    </NuxtLink>
  </div>
</template>

<script setup lang="ts">
definePageMeta({
  layout: 'home'
})
</script>

<style scoped>
.dashboard-box {
  background-color: #e63946;
  color: #fff;
  border-radius: 12px;
  padding: 2rem;
  box-shadow: 0 4px 8px rgb(230 57 70 / 0.3);
  text-align: center;
  min-width: 180px;
  flex-grow: 1;
  transition: transform 0.3s ease;
  cursor: default;
}

.dashboard-box:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 16px rgb(230 57 70 / 0.5);
}

h4 {
  font-weight: 600;
  margin-bottom: 0.5rem;
}

.display-5 {
  font-weight: 700;
}
</style>
