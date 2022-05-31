<script setup lang="ts">
import { RouterView } from 'vue-router'
</script>
<template>
  <main>
    <nav class="navbar navbar-expand-md navbar-light fixed-top bg-light">
      <div class="container-fluid">
        <a class="navbar-brand" href="/">
          <img class="logo" src="/assets/images/logo.png" width="150">
        </a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarCollapse">
          <form class="d-flex  m-auto mb-2 mb-md-0" role="search">
            <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
          </form>

          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="/upload">Upload</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="/login">Login</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="/register">Register</a>
            </li>

          </ul>
        </div>
      </div>
    </nav>

    <div class="container-lg p-lg-3 p-0">
        <RouterView />
  </div>
  </main>

</template>

<style>
@import '../src/App.css';
</style>