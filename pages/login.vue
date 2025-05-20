<!-- pages/login.vue -->
<template>
  <div class="container d-flex justify-content-center align-items-center min-vh-100 bg-white">
    <div class="card p-4 shadow" style="max-width: 400px; width: 100%;">
      <h2 class="text-center text-danger mb-4">Login</h2>
      <form @submit.prevent="handleLogin">
        <div class="mb-3">
          <label for="email" class="form-label text-danger">Email address</label>
          <input
            v-model="email"
            type="email"
            class="form-control"
            id="email"
            placeholder="Enter email"
            required
          />
        </div>
        <div class="mb-3">
          <label for="password" class="form-label text-danger">Password</label>
          <input
            v-model="password"
            type="password"
            class="form-control"
            id="password"
            placeholder="Password"
            required
          />
        </div>
        <button type="submit" class="btn btn-danger w-100">Login</button>
      </form>
    </div>
  </div>
</template>

<script setup lang="ts">

const email = ref('')
const password = ref('')
const router = useRouter()

const handleLogin = async () => {
    router.push('/')
}
</script>
