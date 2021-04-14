<template>
     <!-- rodapé -->
            <div id="footer">
            <footer>
                <article class="art_fot">
                    <p>todos os direitos reservados</p>                                       
                </article>
                <article class="art_fot">
                    <img src="../assets/logo.png" class="img_fot">
                </article>
                <article class="art_fot">
                    <img src="../assets/face.png">
                        <img src="../assets/tt.png">
                        <img src="../assets/insta.png">
                </article>
                
            </footer>
            </div>
</template>

<style scoped> 

    footer{
        
        margin: 0px;
        box-sizing: border-box;
        display: flex;
        background: #A7F5E8;
        color: #000;
        justify-content: space-around;
        position: relative;
        padding: 10px;        
    }   

    @media screen and (max-width:768px){
        footer{
        height: 110%;
        display:grid;
        padding: 20px;
        }

    }
</style>