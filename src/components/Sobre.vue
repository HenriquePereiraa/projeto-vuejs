<template>
  <section class="sobre">
    <div class="container">
        <h2>Sobre nós</h2>

        <div class="sobre-wraper">
            
            <div class="img-sobre"></div><!--img-->

            <div class="texto-sobre">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis eu enim feugiat,
                    lacinia magna vitae, ullamcorper tortor. In pretium tincidunt ex, sit amet vulputate
                    sapien ullamcorper at. Mauris finibus est lectus, sed venenatis dolor egestas quis.
                    Etiam lobortis quam a quam fermentum, sed mattis risus auctor. Integer dictum elementum nisl,
                    tempus lorem consectetur vel. Suspendisse ullamcorper, urna a cursus pretium, turpis augue commodo
                    felis, eget cursus tortor velit sit amet mi.
            </div><!--texto-sobre-->
        </div><!--sobre-wraper-->
    </div><!--container-->   
  </section>
</template>

<script>
export default {
    name:"Sobre"
}
</script>

<style scoped>

    .container{max-width: 1200px; padding: 0 2%; margin:0 auto;}
    section.sobre{
        padding:60px 0;
    }

    .sobre h2{
        margin: 30px 0;
        color:#67AB97;
    }

    .sobre-wraper{
        display: flex;
        flex-wrap: wrap;
        margin-top: 100px;
    }

    .img-sobre{
        width: 50%;
        height: 400px;
        background-image: url("../assets/sobre.jpg");
        background-position: center;
        background-size: cover;
    }

    .texto-sobre{
        width: 50%;
        padding:0 2%;
        line-height: 30px;
        text-align:justify;
    }

    @media screen and (max-width:768px){
        .sobre-wraper{text-align: center;}
        .img-sobre{
            display: inline-block;
            width: 90%;
            margin:0 auto;
        }
        .texto-sobre{
            width: 90%;
            margin: 20px auto;
        }
    }
    
</style>