<template>
  <div id="home">
    <nav-section />
    <div class="titles">
      <h1>Elassal Advantage</h1>
      <h5>Experiences - Aggressive - Results</h5>
    </div>
    <img src="../assets/detroit-courthouse.jpg" alt="">
    <p>The difference at Elassal & Associates is sincere personal attention to your case. Most Lawyers and mega-firms spend their time and resources on advertising to refer your case to unknown Attorneys for an easy referral fee. We are passionate about the law and enjoy getting results for our clients; we diligently spend our time researching and fighting for you! Whether your case is a civil, business, criminal, or auto accident personal injury matter, Lawrence Elassal will work directly with you from the beginning of your case until the end.</p>
    <button>Read More</button>
    <testimonials />
    <contact />
    <location />
  </div>
</template>

<script>
import NavSection from '../NavSection'
import Testimonials from '../Testimonials'
import ContactForm from '../ContactForm'
import LocationSection from '../Location'

export default {
  name: "Home",
  data() {
    return {
      navOpen: true,
      toggleDropdown: false,
      toggleAreas: false
    }
  },
  components: {
    navSection: NavSection,
    testimonials: Testimonials,
    contact: ContactForm,
    location: LocationSection
  }
}
</script>

<style scoped>
  #home {
    font-family: 'Lora', serif;
    text-align: center;
  }

  h5 {
    font-family: 'Open Sans', sans-serif;
    color: #666;
  }

  .titles {
    margin: 20px 0;
  }

  img {
    margin-bottom: 10px;
  }

  p {
    padding: 0 40px;
    text-align: justify;
  }

  button {
    padding: 10px 20px;
    margin: 20px 0 20px 150px;
    /* float: right; */
    background-color: #053D61;
    color: #eee;
    border: none;
  }

  
</style>


