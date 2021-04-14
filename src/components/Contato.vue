<template>
    <div id="Contato">
        <h1>Entre em contato</h1>
        <div id="main_area">
            <form>
                <input type="text" placeholder="Nome">
                <input type="text" placeholder="E-mail">
                <textarea placeholder="deixe uma mensagem"></textarea>
                <button type="submit">enviar</button>
            </form>
            <div>
                <span>Telefone: (99)9999-9999</span><br><br>
                <span>Endereço: Avenida pernambucana, 123 Edificio Stark 3° Andar/Sala 123 - Recife/PE</span>
            </div>
        </div>
    </div>
</template>

<style scoped>
    /* BODY */
    #Contato {
        height: 931px;
        width: 100%;
        background-image: url("../assets/bg_02.png");
        background-repeat: no-repeat;
        background-position: center bottom;
    }
    /* TITULO */
    #Contato > h1 {
        position: relative;
        top: 75px;
        padding-left: 50px;  
        color: #349075;
    }
    /* MAIN AREA */
    #main_area {
        position: relative;
        top: 385px;
        height: 466px;
        width: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    /* MAIN AREA > FORMULÁRIO */
    #main_area > form {
        width: 600px;
        display: flex;
        flex-direction: column;
        border-bottom: 1px solid black;
    }
    #main_area > form input {
        height: 40px;
        width: 600px;
        border-radius: 15px;
        border: 0px;
        padding-inline: 20px;
        margin: 10px 0px 10px 0px;
    }
    #main_area > form textarea {
        height: 100px;
        width: 600px;
        padding: 20px; 
        border-radius: 15px;
        border: 0px;
        margin: 10px 0px 10px 0px;
    }
    #main_area > form button {
        height: 31px;
        width: 140px;
        text-align: center;
        background-color: #31C399;
        color: white;
        border-radius: 15px;
        border: 0px;
        margin: 10px 0px 70px 0px;
    }
    #main_area > div {
        width: 600px;
        padding-top: 5px;
        padding-left: 5px;
        font-size: 16px;
    }
    @media screen and (max-width:768px){
        #main_area > form{
        width: 90%;
        }
        #main_area > form input{
        width: 90%;
        }
        #main_area > form textarea{
            width: 90%;
        }
        #main_area > div{
           width: 90%;
        }
    }
    
</style>