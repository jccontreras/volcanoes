<template>
  <div class="home">
    <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
      <ol class="carousel-indicators">
        <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
        <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
        <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
        <li data-target="#carouselExampleIndicators" data-slide-to="3"></li>
      </ol>
      <div class="carousel-inner">
        <div class="carousel-item active">
          <img src="@/assets/volcano1.jpg" class="d-block w-100">
          <div class="carousel-caption d-none d-md-block">
            <h1 style="font-family: 'Noto Sans CJK SC'">Welcome to the volcanoe's world!!!</h1>
          </div>
        </div>
        <div class="carousel-item">
          <img src="@/assets/volcano2.jpg" class="d-block w-100">
        </div>
        <div class="carousel-item">
          <img src="@/assets/volcano3.jpg" class="d-block w-100">
        </div>
        <div class="carousel-item">
          <img src="@/assets/volcano4.png" class="d-block w-100">
        </div>
      </div>
      <a class="carousel-control-prev" href="#carouselExampleIndicators"
         role="button" data-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
      </a>
      <a class="carousel-control-next" href="#carouselExampleIndicators"
         role="button" data-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
      </a>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
};
</script>
