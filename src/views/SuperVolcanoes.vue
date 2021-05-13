<template>
  <div class="about">
    <div class="jumbotron">
      <h1 class="display-4">What's a Super Volcano</h1>
      <p class="lead">
        Most volcanic eruptions
        produce 1-10 kilometers of material, but supervolcanic eruptions are rare events
        where at least 1000 cubic kilometers of pyroclastic material or at least 450 kilometers
        of magma is ejected during a catastrophic eruption! To get an idea of
        how much magma that is ... remember that the famous Mount St. Helens eruption in 1980
        resulted in only 0.1 cubic kilometers of magma being erupted for at least 9 hours. So a
        supervolcanic eruption could be equivalent to approximately 4500 Santa Helena Mountains
        occurring in 9 hours in an area equal to the city of Los Angeles.When that large amount
        of material leaves a magma chamber underground, what remains near the surface collapses
        to fill in the empty space. The resulting depression on the surface is called a "caldera."
        There is a large concentration of these calderas in the Central Andes,
        shared between Bolivia, Chile and Argentina.
      </p>
      <hr class="my-4">
      <p>This is more amazing information about super volcanoes</p>
      <div class="container">
        <div class="row">
          <div class="col-sm">
            <a class="btn btn-dark btn-lg" href="https://www.youtube.com/watch?v=kAlawvE8lVw"
               role="button" target="_blank" title="Video">National Geographic</a>
          </div>
          <div class="col-sm">
            <a class="btn btn-dark btn-lg" href="https://www.youtube.com/watch?v=LVtNvJPU1wY"
               role="button" target="_blank" title="Video">Most Destructive</a>
          </div>
          <div class="col-sm">
            <a class="btn btn-dark btn-lg" href="https://www.youtube.com/watch?v=hDNlu7Qf6_E"
               role="button" target="_blank" title="Video">Consequences</a>
          </div>
        </div>
      </div>
      <hr class="my-4">
      <h5>These are the super volcanoes of the world</h5>
      <super-volcanoes-component/>
    </div>
  </div>
</template>

<script>
import SuperVolcanoesComponent from '@/components/SuperVolcanoesComponent.vue';

export default {
  name: 'SuperVolcanoes',
  components: {
    SuperVolcanoesComponent,
  },
};
</script>

<style scoped>

</style>
