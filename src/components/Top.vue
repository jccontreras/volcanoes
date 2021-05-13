<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
      <router-link class="nav-link" :to="{name: 'home'}" title="Go Home">
        <img src="@/assets/mylogo2.png" style="max-height: 50px; max-width: 80px"
             @click="changeLk(0)">
      </router-link>
    <button class="navbar-toggler" type="button" data-toggle="collapse"
            data-target="#navbarNav" aria-controls="navbarNav"
            aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav">
        <li id="lk1" class="nav-item" @click="changeLk(1)">
          <router-link class="nav-link" :to="{name: 'about'}">
            About
          </router-link>
        </li>
        <li id="lk2" class="nav-item" @click="changeLk(2)">
          <router-link class="nav-link" :to="{name: 'types'}">
            Types
          </router-link>
        </li>
        <li id="lk3" class="nav-item" @click="changeLk(3)">
          <router-link class="nav-link" :to="{name: 'superv'}">
            Super Volcanoes
          </router-link>
        </li>
      </ul>
      <div class="col" style="text-align: end">
        <span class="navbar-text">
          Made by Ragnarok (Juan Camilo Conteras Chacon)
        </span>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Top',
  methods: {
    changeLk(codlk) {
      if (codlk === 0) {
        document.getElementById('lk1').className = 'nav-item';
        document.getElementById('lk2').className = 'nav-item';
        document.getElementById('lk3').className = 'nav-item';
      } else if (codlk === 1) {
        document.getElementById('lk1').className = 'nav-item active';
        document.getElementById('lk2').className = 'nav-item';
        document.getElementById('lk3').className = 'nav-item';
      } else if (codlk === 2) {
        document.getElementById('lk1').className = 'nav-item';
        document.getElementById('lk2').className = 'nav-item active';
        document.getElementById('lk3').className = 'nav-item';
      } else if (codlk === 3) {
        document.getElementById('lk1').className = 'nav-item';
        document.getElementById('lk2').className = 'nav-item';
        document.getElementById('lk3').className = 'nav-item active';
      }
    },
  },
};
</script>
