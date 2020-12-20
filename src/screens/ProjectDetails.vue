<template>
  <div>
    <header>Proeject Details</header>
    <p>start planning your space today!</p>

    <form id="project-form">
      <div class="project-name">
        <label for="input-name" class="lbl-name">Project Name</label>
        <input type="text" id="input-name" name="name" v-model="name" />
        <p class="name-descr">Enter a name for your project</p>
      </div>
      <div class="project-type">
        <label for="radio-type" class="lbl-name">Project Type</label>
        <input type="radio" id="type-select" name="type" v-model="type" />
        <input type="radio" id="type-driveway" name="type" v-model="type" />
        <input type="radio" id="type-patio" name="type" v-model="type" />
        <input type="radio" id="type-pool-deck" name="type" v-model="type" />
        <input
          type="radio"
          id="type-sidewalk_path"
          name="type"
          v-model="type"
        />
      </div>
      <div class="project-square_footage">
        <label for="input-square" class="lbl-square">Square Footage</label>
        <input type="number" id="input-name" name="name" v-model="square" />
        <p class="square-descr">
          Total square footage of the project including borders and accents for
          the calculation.
        </p>
      </div>
      <div class="project-length">
        <label for="input-length" class="lbl-length"
          >Length Restrained (Lineal Ft)</label
        >
        <input type="number" id="input-length" name="length" v-model="length" />
        <p class="length-descr">Enter a name for your project</p>
      </div>
      <div class="project-baserock">
        <label for="input-baserock" class="lbl-baserock"
          >Base Rock (Inches)
        </label>
        <input
          type="number"
          id="input-baserock"
          name="baserock"
          v-model="baserock"
        />
        <p class="baserock-descr">
          Quantity shown is based on ICPI suggested amounts for your project.
          You may require more or less. Adjust at your own risk.
        </p>
      </div>
      <div class="project-waste">
        <label for="input-waste" class="lbl-waste">Waste Overage (%) </label>
        <input type="number" id="input-waste" name="waste" v-model="waste" />
        <p class="waste-descr">
          We recommend 5% of waste overage to account for damaged product or
          non-linear patio or walkway designs.
        </p>
      </div>
      <div class="project-descr">
        <label for="input-descr" class="lbl-descr">Project Description </label>
        <input type="text-area" id="input-name" name="descr" v-model="descr" />
      </div>
      <button>get started</button>
    </form>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped></style>
