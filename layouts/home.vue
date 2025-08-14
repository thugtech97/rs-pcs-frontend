<template>
  <div class="d-flex min-vh-100 bg-light">
    <!-- Sidebar -->
    <nav class="sidebar bg-dark text-light d-flex flex-column p-3">
      <div class="mb-4">
        <h4 class="text-white">Rapid Screening</h4>
      </div>
      <ul class="nav nav-pills flex-column gap-2">
        <li class="nav-item">
          <a href="#" class="nav-link active d-flex align-items-center gap-2">
            <span class="btn btn-sm btn-danger rounded-pill text-light">Dashboard</span>
          </a>
        </li>
        <li><a href="#" class="nav-link text-light">Settings</a></li>
        <li><a href="#" class="nav-link text-light">Resources</a></li>
        <li><a href="#" class="nav-link text-light">Logout</a></li>
      </ul>
      <div class="mt-auto p-3 bg-danger rounded text-light d-flex justify-content-between align-items-center">
        <div>
          <strong>Visit our site</strong><br />
        </div>
        <button class="btn btn-sm btn-light rounded-circle">
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" viewBox="0 0 16 16">
            <path fill-rule="evenodd" d="M8 12a.5.5 0 0 0 .5-.5V5.707l2.146 2.147a.5.5 0 0 0 .708-.708l-3-3-.007-.007a.498.498 0 0 0-.697.007l-3 3a.5.5 0 1 0 .708.708L7.5 5.707V11.5A.5.5 0 0 0 8 12z"/>
          </svg>
        </button>
      </div>
    </nav>

    <!-- Main Content -->
    <main class="flex-grow-1 p-4">
      <slot />
    </main>
  </div>
</template>

<style scoped>
.sidebar {
  width: 280px;
  border-radius: 12px;
  margin: 20px;
  display: flex;
  flex-direction: column;
  background: #222430;
}

.nav-link.active {
  background-color: #e63946 !important; /* red */
  color: #222430 !important;
  font-weight: 600;
  border-radius: 30px;
  padding: 10px 20px;
}

.nav-link {
  border-radius: 30px;
  padding: 10px 20px;
  transition: background-color 0.3s ease;
}

.nav-link:hover {
  background-color: #e63946;
}

.bg-danger {
  background-color: #e63946 !important;
}

.btn-danger {
  background-color: #e63946 !important;
  font-weight: 600;
}
</style>
