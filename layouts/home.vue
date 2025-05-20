<template>
  <div class="d-flex flex-column min-vh-100 bg-light">
    <!-- Header -->
    <nav class="navbar navbar-expand-lg navbar-dark bg-danger shadow-sm">
      <div class="container-fluid">
        <button
          class="btn btn-outline-light d-lg-none"
          type="button"
          data-bs-toggle="offcanvas"
          data-bs-target="#sidebar"
          aria-controls="sidebar"
        >
          ☰
        </button>
        <a class="navbar-brand" href="#">Rapid Screening - Police Check System</a>
      </div>
    </nav>

    <div class="d-flex flex-grow-1">
      <!-- Sidebar for large screens -->
      <aside class="d-none d-lg-block bg-danger text-white p-3" style="width: 250px;">
        <ul class="nav flex-column">
          <li class="nav-item">
            <NuxtLink class="nav-link text-white" to="/">Dashboard</NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink class="nav-link text-white" to="/login">Settings</NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink class="nav-link text-white" to="/login">Resources</NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink class="nav-link text-white" to="/login">Log out</NuxtLink>
          </li>
        </ul>
      </aside>

      <!-- Sidebar offcanvas for mobile -->
      <div
        class="offcanvas offcanvas-start bg-danger text-white"
        tabindex="-1"
        id="sidebar"
        aria-labelledby="sidebarLabel"
      >
        <div class="offcanvas-header">
          <h5 class="offcanvas-title" id="sidebarLabel">Menu</h5>
          <button
            type="button"
            class="btn-close btn-close-white"
            data-bs-dismiss="offcanvas"
            aria-label="Close"
          ></button>
        </div>
        <div class="offcanvas-body">
          <ul class="nav flex-column">
            <li class="nav-item">
              <NuxtLink class="nav-link text-white" to="/">Dashboard</NuxtLink>
            </li>
            <li class="nav-item">
              <NuxtLink class="nav-link text-white" to="/login">Settings</NuxtLink>
            </li>
            <li class="nav-item">
              <NuxtLink class="nav-link text-white" to="/login">Resources</NuxtLink>
            </li>
            <li class="nav-item">
              <NuxtLink class="nav-link text-white" to="/login">Log out</NuxtLink>
            </li>
          </ul>
        </div>
      </div>

      <!-- Main content -->
      <main class="flex-grow-1 p-4 bg-white shadow-sm">
        <slot />
      </main>
    </div>

    <!-- Footer -->
    <footer class="bg-danger text-white text-center py-3 mt-auto">
      &copy; 2025 Rapid Screening. All rights reserved.
    </footer>
  </div>
</template>
