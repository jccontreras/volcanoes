<template>
  <div class="accordion" id="accordionExample">
    <div class="card" style="background-color: #d4dacc">
      <div class="card-header" id="headingOne">
        <h2 class="mb-0">
          <button class="btn btn-block text-left" type="button" data-toggle="collapse"
                  data-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne"
                  style="color: #2c3e50">
            <img src="@/assets/mylogo.png" style="max-height: 30px; max-width: 60px">
            Types of Volcanoes
          </button>
        </h2>
      </div>

      <div id="collapseOne" class="collapse show" aria-labelledby="headingOne"
           data-parent="#accordionExample" style="background-color: #e9ecef">
        <div class="card-body">
          <div class="container">
            <div class="row">
              <div class="col">
                <div class="card" style="width: 18rem;">
                  <img src="@/assets/estravolc.jpg" class="card-img-top" style="max-height: 200px">
                  <div class="card-body">
                    <h5 class="card-title">Composite volcanoes or Stratovolcano</h5>
                    <p class="card-text" v-if="see1">
                      They are large and have a conical shape with a central crater,
                      the volcanic building is formed by successive layers of lava deposits
                      and rock fragments: slag, sand and ash, the product of different
                      eruptions. For this reason they are called compound. These volcanoes
                      often form impressive snow-capped peaks that are greater than 2,500
                      meters (8.6 miles) in height, 1,000 (621 miles) square kilometers in
                      surface, and 400 kilometers (249 cubic miles) in volume. Composite
                      volcanoes erupt explosively from viscous magma. When magma is very
                      viscous, it rises to the surface, but it clogs the crater and the gas
                      is trapped. Therefore, the pressure will increase and result in an explosive
                      eruption. These volcanoes are located along the subduction zones.
                    </p>
                    <p v-else>
                      They are large and have a conical shape with a central...
                    </p>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(1)" v-if="see1">Close</a>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(1)" v-else>See more</a>
                  </div>
                </div>
              </div>
              <div class="col">
                <div class="card" style="width: 18rem;">
                  <img src="@/assets/caldera.jpg" class="card-img-top" style="max-height: 200px">
                  <div class="card-body">
                    <h5 class="card-title">Boilers</h5>
                    <p class="card-text" v-if="see2">
                      They are the result of large eruptions, which cause the central
                      part or the entire volcanic building to collapse or collapse,
                      leaving a large crater or caldera.
                    </p>
                    <p v-else>
                      They are the result of large eruptions, which cause the central...
                    </p>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(2)" v-if="see2">Close</a>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(2)" v-else>See more</a>
                  </div>
                </div>
              </div>
              <div class="col">
                <div class="card" style="width: 18rem;">
                  <img src="@/assets/escudo.jpg" class="card-img-top" style="max-height: 200px">
                  <div class="card-body">
                    <h5 class="card-title">Volcanoes in Escudo</h5>
                    <p class="card-text" v-if="see3">
                      They are characterized by being large mountains, with gentle
                      slopes, formed by the superposition of flowing lava rivers.
                      Shield volcanoes are huge in size. They are made up of many layers
                      of lava flows. Lava spills out of a central vent or group of vents.
                      It forms a fairly wide cone. It is caused by basaltic lava, which is
                      very fluid, and cannot pile up in steep places. Shield volcanoes can be
                      produced by hot spots that are far from the edges of tectonic plates.
                      They also occur along the mid-oceanic ridge, where seafloor expansion
                      is ongoing, and around areas of subduction related to volcanic arcs.
                      Shield volcano eruptions are characterized by low-explosive lava that
                      forms cinder cones and cones on the vents.
                    </p>
                    <p v-else>
                      They are characterized by being large mountains, with...
                    </p>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(3)" v-if="see3">Close</a>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(3)" v-else>See more</a>
                  </div>
                </div>
              </div>
            </div>
            <div class="row">
              <div class="col">
                <div class="card" style="width: 18rem;">
                  <img src="@/assets/cupula.jpg" class="card-img-top" style="max-height: 200px">
                  <div class="card-body">
                    <h5 class="card-title">Lava Dome</h5>
                    <p class="card-text" v-if="see4">
                      They present smaller structures, compared to the previous
                      ones, with steep slopes and product of the accumulation of very
                      viscous lavas and flows of blocks and incandescent ash.
                    </p>
                    <p v-else>
                      They present smaller structures, compared to the...
                    </p>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(4)" v-if="see4">Close</a>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(4)" v-else>See more</a>
                  </div>
                </div>
              </div>
              <div class="col">
                <div class="card" style="width: 18rem;">
                  <img src="@/assets/cono.jpg" class="card-img-top" style="max-height: 200px">
                  <div class="card-body">
                    <h5 class="card-title">Cinder Cone or Slag</h5>
                    <p class="card-text" v-if="see5">
                      They are relatively small cones that, as their name indicates, are formed
                      by the accumulation of ash and slag. An cinder cone is a steep conical
                      hill formed above a vent. Cinder cones are some of the most common volcanic
                      formations found in the world. They are not very famous, as their eruptions
                      generally do not cause any loss of life. Cinder cones are primarily made up
                      of strombolian eruptions, which occur when magma is viscous, and the
                      trapped gas intermittently escapes as it rises to the surface. This often
                      results in blocks and bombs falling on the surrounding environment.
                      Cones usually grow in groups and occur on the slopes of volcanoes and
                      stratum-shield volcanoes.
                      Cinder cones are built from fragments of lava called ashes. Lava fragments
                      are expelled from a single vent and accumulate around the vent as they fall
                      back to earth. Cinder cones grow rapidly and approach their maximum size in
                      a short time. These rarely exceed 250 meters (820 feet) in height and 500
                      meters (1,640 feet) in diameter. Its form can be modified during its (short)
                      life. A great example of a cinder cone is the Paricutín in Mexico
                    </p>
                    <p v-else>
                      They are relatively small cones that, as their name...
                    </p>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(5)" v-if="see5">Close</a>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(5)" v-else>See more</a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="card" style="background-color: #d4dacc">
      <div class="card-header" id="headingTwo">
        <h2 class="mb-0">
          <button class="btn btn-block text-left collapsed"
                  type="button" data-toggle="collapse"
                  data-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo"
                  style="color: #2c3e50">
            <img src="@/assets/mylogo.png" style="max-height: 30px; max-width: 60px">
            Types of Rashes
          </button>
        </h2>
      </div>
      <div id="collapseTwo" class="collapse" aria-labelledby="headingTwo"
           data-parent="#accordionExample" style="color: #2c3e50">
        <div class="card-body">
          <div class="container">
            <div class="row">
              <div class="col">
                <div class="card" style="width: 18rem;">
                  <img src="@/assets/rash1.jpg" class="card-img-top" style="max-height: 200px">
                  <div class="card-body">
                    <h5 class="card-title">Hawaiian</h5>
                    <p class="card-text" v-if="see6">
                      The volcano emits a slightly viscous lava, quite fluid,
                      since it does not have many pyroclastic materials
                      (hot mixture of gases, ash and rock fragments. The gases are released
                      little by little, and therefore, the explosions are minimal.
                    </p>
                    <p v-else>
                      the volcano emits a slightly viscous lava, quite fluid...
                    </p>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(6)" v-if="see6">Close</a>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(6)" v-else>See more</a>
                  </div>
                </div>
              </div>
              <div class="col">
                <div class="card" style="width: 18rem;">
                  <img src="@/assets/rash2.jpg" class="card-img-top" style="max-height: 200px">
                  <div class="card-body">
                    <h5 class="card-title">Strombolian</h5>
                    <p class="card-text" v-if="see7">
                      The volcano releases pyroclastic material. The explosions
                      are sporadic and the volcano does not emit lava continuously.
                    </p>
                    <p v-else>
                      the volcano releases pyroclastic material. The explosions...
                    </p>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(7)" v-if="see7">Close</a>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(7)" v-else>See more</a>
                  </div>
                </div>
              </div>
              <div class="col">
                <div class="card" style="width: 18rem;">
                  <img src="@/assets/rash3.jpg" class="card-img-top" style="max-height: 200px">
                  <div class="card-body">
                    <h5 class="card-title">Vulcaniana</h5>
                    <p class="card-text" v-if="see8">
                      The volcano emits very viscous lava, little fluid, which solidifies quickly.
                      Large clouds of pyroclastic material form and a lot of ash is emitted.
                      They are characterized by producing a cloud-like eruption similar to a
                      mushroom or fungus. Activity usually begins with a phreatic eruption that
                      discharges debris. The main phase usually consists of an eruption of viscous
                      magma, rich in volcanic gases and forming a dark cloud.
                    </p>
                    <p v-else>
                      The volcano emits very viscous lava, little fluid, which solidifies quickly.
                      Large clouds of...
                    </p>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(8)" v-if="see8">Close</a>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(8)" v-else>See more</a>
                  </div>
                </div>
              </div>
            </div>
            <div class="row">
              <div class="col">
                <div class="card" style="width: 18rem;">
                  <img src="@/assets/rash4.jpeg" class="card-img-top" style="max-height: 200px">
                  <div class="card-body">
                    <h5 class="card-title">Pliniana or Vesuviano</h5>
                    <p class="card-text" v-if="see9">
                      The volcano emits very viscous lava and the explosion is
                      violent. It is characterized by its exceptional strength,
                      continuous gas eruption and the expulsion of large amounts of ash.
                      Sometimes the expulsion of magma is such that the summit of the volcano
                      collapses and produces a caldera. During a Plinian eruption,
                      fine ash can be dispersed over large areas. The Plinian eruptions
                      are named after the famous Roman naturalist, Pliny the Elder, who died
                      during an eruption of Vesuvius in 79 AD.
                    </p>
                    <p v-else>
                      The volcano emits very viscous lava and the explosion is...
                    </p>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(9)" v-if="see9">Close</a>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(9)" v-else>See more</a>
                  </div>
                </div>
              </div>
              <div class="col">
                <div class="card" style="width: 18rem;">
                  <img src="@/assets/rash5.jpg" class="card-img-top" style="max-height: 200px">
                  <div class="card-body">
                    <h5 class="card-title">Peleano</h5>
                    <p class="card-text" v-if="see10">
                      The volcano is named after the 1902 Mount Pelee eruption in Martinique
                      in which thousands of people died. The lava quickly consolidates and a
                      plug is produced in the crater. As the gases have no outlet, great pressure
                      is created inside the volcano so the walls come to give way and the lava
                      is expelled from the sides of the volcanoes.
                    </p>
                    <p v-else>
                      The volcano is named after the 1902 Mount Pelee eruption in...
                    </p>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(10)" v-if="see10">Close</a>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(10)" v-else>See more</a>
                  </div>
                </div>
              </div>
              <div class="col">
                <div class="card" style="width: 18rem;">
                  <img src="@/assets/rash6.jpeg" class="card-img-top" style="max-height: 200px">
                  <div class="card-body">
                    <h5 class="card-title">Hydro-Volcanic</h5>
                    <p class="card-text" v-if="see11">
                      They are eruptions that are generated by the interaction
                      of magma with groundwater or surface water. They are the
                      "liquid: equivalent of a Strombolian eruption, although they
                      are more explosive.
                    </p>
                    <p v-else>
                      They are eruptions that are generated by the interaction...
                    </p>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(11)" v-if="see11">Close</a>
                    <a href="#" class="btn btn-primary"
                       @click="openOrClose(11)" v-else>See more</a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Types',
  data() {
    return {
      see1: false,
      see2: false,
      see3: false,
      see4: false,
      see5: false,
      see6: false,
      see7: false,
      see8: false,
      see9: false,
      see10: false,
      see11: false,
    };
  },
  methods: {
    openOrClose(codsee) {
      if (codsee === 1) {
        this.see1 = !this.see1;
      } else if (codsee === 2) {
        this.see2 = !this.see2;
      } else if (codsee === 3) {
        this.see3 = !this.see3;
      } else if (codsee === 4) {
        this.see4 = !this.see4;
      } else if (codsee === 5) {
        this.see5 = !this.see5;
      } else if (codsee === 6) {
        this.see6 = !this.see6;
      } else if (codsee === 7) {
        this.see7 = !this.see7;
      } else if (codsee === 8) {
        this.see8 = !this.see8;
      } else if (codsee === 9) {
        this.see9 = !this.see9;
      } else if (codsee === 10) {
        this.see10 = !this.see10;
      } else if (codsee === 11) {
        this.see11 = !this.see11;
      }
    },
  },
};
</script>
