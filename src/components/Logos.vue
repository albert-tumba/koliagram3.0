<template>
  <div class="logos">
    <img src="@/assets/logo-otacos-black.png" class="logo-1" />
    <img src="@/assets/logo-chickenspot-black.png" class="logo-2" />
    <img src="@/assets/logo-wffactory-black.png" class="logo-3" />
    <img src="@/assets/logo-obrooklyn-black.png" class="logo-4" />
  </div>
</template>

<script>
export default {
  name: "Logos",
};
</script>

<style scoped>
.logos {
  margin-left: auto;
  margin-right: auto;
  width: 1035px;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.logo-1 {
  width: 9.375rem; /*150px*/
  height: 9.375rem; /*150px*/
}

.logo-2 {
  width: 200px;
  height: 200px;
}

.logo-3 {
  width: 200px;
  height: 200px;
}

.logo-4 {
  width: 200px;
  height: 200px;
}

@media screen and (max-width: 960px) {
  .logos {
    width: 100%;
  }

  .trust-section {
    display: flex;
    flex-direction: row;
  }

  .logos {
    display: flex;
    flex-direction: row;
  }

  .logo-1 {
    width: 90px;
    height: 90px;
  }

  .logo-2 {
    width: 100px;
    height: 100px;
  }

  .logo-3 {
    width: 90px;
    height: 90px;
  }

  .logo-4 {
    width: 90px;
    height: 90px;
  }
}
</style>