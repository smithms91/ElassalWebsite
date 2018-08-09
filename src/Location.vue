<template>
  <div id="location">
    <h1>Office Location</h1>
    <p class="description">The Elassal & Associates Team is pleased to announce the opening of our brand new Dearborn office conveniently located on Telegraph Road near Ford Road.</p>
    <div class="findus">
      <img class="building" src="./assets/location.png" alt="">
      <div class="address">
        <p>1000 North Telegraph Road</p>
        <p>Dearborn, MI</p>
        <p>48128</p>
        <p>(313) 529-4357</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Location",
  data() {
    return {

    }
  }
}
</script>

<style scoped>
  #location {
    padding: 10px;
  }

  h1 {
    margin-bottom: 20px;
  }

  .building {
   width: 150px;
   height: 100px;
  }

  .map {
    width: 100%;
    margin-top: 40px;
  }

  .findus {
    display: flex;
    align-items: center;
    justify-content: space-around;
    margin-bottom: 40px;
  }

  .address p {
    font-size: 12px;
    text-align: center;
  }

  .description {
    margin-bottom: 20px;
  }
 
</style>


