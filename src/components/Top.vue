<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <router-link class="nav-link" :to="{name: 'home'}" title="Go Home">
        <img src="@/assets/mylogo2.png" style="max-height: 50px; max-width: 80px">
      </router-link>
    <button class="navbar-toggler" type="button" data-toggle="collapse"
            data-target="#navbarNav" aria-controls="navbarNav"
            aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li class="nav-item active">
          <router-link class="nav-link" :to="{name: 'about'}">
            About
          </router-link>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Features</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Pricing</a>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
        </li>
      </ul>
      <div class="col" style="text-align: end">
        <span class="navbar-text">
          Made by Ragnarok
        </span>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Top',
};
</script>
