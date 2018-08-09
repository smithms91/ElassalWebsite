<template>
  <div id="contact-form">
    <h1>Contact Us</h1>
    <form>
      <label for="name">Name *</label>
      <input type="text" placeholder="First Last">
      <label for="name">Phone *</label>
      <input type="text" placeholder="(123) 456-7890">
      <label for="name">Email *</label>
      <input type="text" placeholder="email@gmail.com">
      <label for="name">Message *</label>
      <textarea type="text" placeholder="Enter Message"></textarea>
      <button>Submit</button>
    </form>
  </div>
</template>

<script>
export default {
  name: "Contact",
  data() {
    return {

    }
  }
}
</script>

<style scoped>
  #contact-form {
    padding: 40px 20px;
    background-image: url('./assets/testimonialbg.png');
    background-size: cover;
    background-position: center right;
    color: #eee;
  }

  #contact h1 {
    margin-bottom: 20px;
  }

  form {
    width: 250px;
    margin: 0 auto;
  }

  label {
    display: block;
    text-align: left;
    margin-bottom: 5px;
    
  }

  input, textarea {
    width: 100%;
    margin-bottom: 10px;
    padding: 10px 20px;
    border-radius: 5px;
    border: 1px solid black;
    font-family: 'Open Sans', sans-serif;
  }

  button {
    padding: 20px 40px;
    margin-top: 20px;
    border-radius: 5px;
    border: none;
    background-color: #053D61;
    border: 2px solid rgb(40, 61, 75);
    color: #eee;
  }
 
</style>


