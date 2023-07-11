<script>
  export let currentPage;
</script>

<style>
  .Contacts{
    display: flex;
    margin-left: 10%;

  }
  .facbookIconAn,.TwitterIconAn,.GetHupIconAn,.LinkedIniconAn{
    width: 30px;
    margin-left: 6%;

    transition: all 0.6S;
  }
  .TwittterIconContainer,.facbookIconsContainer,.GetHuoIconContainer,.LinkedInIconContainer{
    width: 100%;
  }
  .facbookIcon,.LinkedInIcon,.TwitterIcon,.GetHUPIcon{
    width:100%;
  }



  .navigation{
    margin-top:-10px ;
    display: flex;
    align-items: center;
    justify-content: space-around;
    z-index: 111;


  ;
  }
  .logo{
    font-weight: 800;
    letter-spacing: 3px;
    font-family: Candara;
    display: flex;
    font-size: 20px;

  }
  .nav-pages{
    display: flex;

  }
  li a{
    transition: all 1s;
    color: Black;
    font-family: Arial;
    font-size: 18px;
    font-weight: 600;

  }
  li:hover a {
    text-shadow: 5px 5px 3px rgba(0,0,0,0.4);

  }

  .LinkedIniconAn:hover ,.facbookIconAn:hover,.TwitterIconAn:hover,.GetHupIconAn:hover {


    opacity: 0.2;

  }

  li{
    list-style: none;
  }
  li a{
    text-decoration: none;

    margin-right: 10px;


  }

</style>

<nav class="navigation">
  <div class="logo">Hamza Aldaghstany</div>
  <ul class="nav-pages">
    <li><a href="#">Home</a></li>
    <li><a href="#">About</a></li>
    <li><a href="#">Skills</a></li>
  </ul>
  <div class="Contacts">
    <a href="#" class="facbookIconAn">
      <div class="facbookIconsContainer">
        <img src="img/icons/facebook-svgrepo-com.svg" class="facbookIcon">
      </div>

    </a>
    <a href="#" class="LinkedIniconAn">
      <div class="LinkedInIconContainer">
        <img src="img/icons/linkedin-svgrepo-com.svg" class="LinkedInIcon">
      </div>

    </a>
    <a href="#" class="TwitterIconAn">
      <div class="TwittterIconContainer">
        <img src="img/icons/twitter-svgrepo-com.svg" class="TwitterIcon">
      </div>

    </a>
    <a href="#" class="GetHupIconAn">
      <div class="GetHuoIconContainer">
        <img src="img/icons/github-svgrepo-com.svg" class="GetHUPIcon">
      </div>

    </a>
  </div>
</nav>
