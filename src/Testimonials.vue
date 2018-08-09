<template>
  <div id="testimonial">
    <h1>Testimonials</h1>
    <carousel :per-page="1" :autoplay="true" :autoplay-timeout="5000" :loop="true" :pagination-active-color="'#053D61'">
      <slide>
        <div class="test">
          <p class="message">A true fighter!!</p>
          <p class="author">&ndash; Mike Manollo</p>
        </div>
      </slide>
      <slide>
        <div class="test">
          <p class="message">All the Attorneys are very helpful.</p>
          <p class="author">&ndash; Lisa G</p>
        </div>
      </slide>
      <slide>
        <div class="test">
          <p class="message">Thanks!! We won our case!! </p>
          <p class="author">&ndash; Anthony Neal</p>
        </div>
      </slide>
    </carousel>
  </div>
</template>

<script>
export default {
  name: "Testimonials",
  data() {
    return {

    }
  }
}
</script>

<style scoped>
  #testimonial {
    font-family: 'Merriweather', serif;
    background-color: #999;
    padding: 80px 0 40px 0;
    clip-path: polygon(0 20%, 100% 0, 100% 100%, 0 100%);
    color: #eee;
  }

  #testimonial h1 {
    margin-bottom: 40px;
  }

  .test {
    box-shadow: inset 1px 1px 5px black;
    border-radius: 5px;
    width: 250px;
    margin: 0 auto;
    padding: 20px;
  }

  .message {
    margin-bottom: 10px;
    
  }

  .author {
    font-size: 14px;
    font-family: 'Open Sans', sans-serif;
  }
</style>


