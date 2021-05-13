<template>
  <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
    <ol class="carousel-indicators">
      <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
      <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
      <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
      <li data-target="#carouselExampleIndicators" data-slide-to="3"></li>
    </ol>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="@/assets/sv1.jpg" class="d-block w-100">
        <div class="carousel-caption d-none d-md-block">
          <p class="lead" style="font-family: 'Noto Sans CJK SC'; color: antiquewhite">
            Yellowstone is considered a super volcano despite the fact that it has not erupted for
            640 million years, however it is considered by scientists as a lethal threat to
            humanity because it still It is active.
          </p>
        </div>
      </div>
      <div class="carousel-item">
        <img src="@/assets/sv2.jpg" class="d-block w-100">
        <div class="carousel-caption d-none d-md-block">
          <p class="lead" style="font-family: 'Noto Sans CJK SC'; color: antiquewhite">
            The volcano Vesuvius is known for the devastation that it caused to a city, Pompeii,
            that's right, this is the volcano that in the year 79 destroyed several cities,
            including Herculaneum and Pompeii that were buried under lava and were a
            legend for centuries
          </p>
        </div>
      </div>
      <div class="carousel-item">
        <img src="@/assets/sv3.jpg" class="d-block w-100">
        <div class="carousel-caption d-none d-md-block">
          <p class="lead" style="font-family: 'Noto Sans CJK SC'; color: antiquewhite">
            The Calbuco volcano is one of the three most dangerous volcanoes in Chile,
            in fact it is classified as one of the most explosive, its last eruption that
            it registered reached a rank 4 of the Volcano Explosivity Index and caused an
            ash column about 17 kilometers high.
          </p>
        </div>
      </div>
      <div class="carousel-item">
        <img src="@/assets/sv4.jpg" class="d-block w-100">
        <div class="carousel-caption d-none d-md-block">
          <p class="lead" style="font-family: 'Noto Sans CJK SC'; color: antiquewhite">
            The Merapi volcano is considered one of the most dangerous since it is in
            continuous eruption, even the last one occurred in May 2018. It is located
            in Indonesia. It also tends to erupt with pyroclastic flows, avalanches
            of fiery gas and volcanic material that sweep down the slopes at hundreds
            of kilometers per hour.
          </p>
        </div>
      </div>
      <div class="carousel-item">
        <img src="@/assets/sv5.jpg" class="d-block w-100">
        <div class="carousel-caption d-none d-md-block">
          <p class="lead" style="font-family: 'Noto Sans CJK SC'; color: antiquewhite">
            Another dangerous volcano found in Indonesia is Krakatoa, which in 1883 was
            able to destroy a large part of the island that contained it; it was the largest
            eruption of which certain news is had.
          </p>
        </div>
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
</template>

<script>
export default {
  name: 'SuperVolcanoesComponent',
};
</script>
