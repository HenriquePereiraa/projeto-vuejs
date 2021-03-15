<template>
<section>
    <header>
      <img src="../assets/logo.png" alt="Logo">
      <nav class="desktop">
          <ul>
              <li><a href="#">Sobre nós</a></li>
              <li><a href="#">Serviços</a></li>
              <li><a href="#">Depoimentos</a></li>
              <li><a href="#">Contato</a></li>
          </ul>
      </nav><!--desktop-->

      <!-- TODO: menu mobile -->
      <div class="clear"></div>
  </header> 
  
  <div class="banner">
    <div class="container">
        <div class="one">
            <h2>Seu sorriso perfeito através de um tratamento discreto e inovador em Recife.</h2>

            <form>
                <input type="email" name="email" placeholder="E-mail">
                <input type="submit" value="Agende uma avaliação">
            </form>
            <span>Ou ligue para agendar (99)9999-9999</span>
        </div><!--one-->

        <div class="two">
            <img src="../assets/circle01.png" alt="img1">
            <img src="../assets/circle02.png" alt="img1">
            <img src="../assets/circle03.png" alt="img1">
            <img src="../assets/circle04.png" alt="img1">
        </div><!--two-->

        <div class="clear"></div>
    </div><!--container-->
  </div><!--banenr-->

</section>
  
</template>

<script>
export default {
    name:"Banner"
}
</script>

<style scoped>

    .clear{clear: both;}
    .container{max-width:1280px; padding:0 2%; margin:0 auto;}

    header{
        background-color: #9AE4CF;
        padding:10px 2%;
        position: fixed;
        width: 100%;
        z-index: 9999;
    }
    header > img{
        width:120px;
        cursor: pointer;
    }
    nav.desktop{
        float: right;
        margin-top: 10px;
    }
    nav.desktop li{
        display: inline-block;
        margin:0 15px;
    }
    nav.desktop a{
        text-decoration: none;
        color:white;
        font-size: 17px;
        font-weight: normal;
    }

    @media screen and (max-width:768px){
        nav.desktop{display: none;}
    }
    /*section banner*/

    div.banner{
        width: 100%;
        min-height: 700px;
        background-image: url('../assets/bg_01.png');
        background-position: center;
    }
    .container{
        position:absolute;
        top:30%;
        left: 10%;
    }
    
    .one{
        width:60%;
        float: left;
        padding:0 30px;
    }

    .one h2{
        color:#0F7053;
        font-weight: bold;
    }

    .one form input[type="email"]{
        width: 300px;
        height: 35px;
        margin-top: 40px;
        line-height: 35px;
        padding-left: 15px;
        border:0;
        border-radius: 10px;
        outline: none;
        display: block;
    }
    .one form input[type="submit"]{
        padding:5px 15px;
        margin-top:8px;
        background-color: #31C399;
        color:white;
        border:0;
        border-radius: 10px;
        outline: none;
        cursor: pointer;
        display: block;
    }

    .one span{
        font-size: 12px;
        font-weight: normal;
    }

    .two{
        float: left;
        width: 40%;
        padding: 0 30px;

    }

    .two img{
        float: left;
        width: 50%;
        border:5px solid transparent; 
        padding:2%;  
    }

    @media screen and (max-width:780px){
        .banner .one{
            width: 100%;
        }
        .banner .two{
            display: none;
        }

        .one h2{font-size: 22px;}
        form{
            margin-top:50px;
        }
        .one form input[type="email"]{
            width:50%;
        }        
    }
    @media screen and (max-width:500px){
        .one form input[type="email"]{
            width:100%;
        } 
    }
</style>