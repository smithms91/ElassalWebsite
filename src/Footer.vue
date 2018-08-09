<template>
  <div id="footer-section">
    <h1>Folow us on Social Media!</h1>
    <ul>
      <li><a href="https://www.facebook.com/pages/Elassal-Associates/730477993696784?timeline_context_item_type=intro_card_work&timeline_context_item_source=100000524897914&fref=tag"><i class="fab fa-facebook-f"></i></a></li>
      <li><a href="https://twitter.com/313lawhelp"><i class="fab fa-twitter"></i></a></li>
      <li><a href="https://www.linkedin.com/feed/"><i class="fab fa-linkedin"></i></a></li>
    </ul>
    <p class="copyright">Copyright &copy; 2018 Elassal and Associates</p>
    <p class="poweredby">Website Powered by <a href="#">Fisher Media</a></p>
  </div>
</template>

<script>
export default {
  name: "FooterSection",
  data() {
    return {

    }
  }
}
</script>

<style scoped>
  #footer-section {
    background-color: #111;
    color: #eee;
  }

  h1 {
    font-size: 20px;
    text-align: center;
    padding-top: 20px;
    font-family: 'Open Sans', sans-serif;
  }

  ul {
    display: flex;
    justify-content: center;
    align-items: center;
    list-style-type: none;
  }

  ul li i {
    margin: 20px;
  }

  ul li:hover i {
    color: #053D61;
  }

  .copyright {
    text-align: center;
    font-family: 'Merriweather', serif;
    border-top: 1px solid rgba(255,255,255,0.5);
    padding: 20px;
    font-size: 12px;
  }

  .poweredby {
    font-family: 'Open Sans', sans-serif;
    text-align: center;
    border-top: 1px solid rgba(255,255,255,0.5);
    padding: 20px;
    font-size: 14px;
  }

  a {
    color: #eee;
  }

  a:hover {
    color: #053D61;
  }


 
</style>


