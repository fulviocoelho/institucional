<template>
    <section class="contato">
        <p class="section-title">Contato</p>
        <p class="section-subtitle">Tem alguma duvida ou gostaria de trabalhar conosco? Entre em contato</p>
        <div class="clear"></div>
        <div class="form">
            <form action="#" @submit="submit">
                <input class="left" type="text" name="nome">
                <input class="right" type="email" name="email">
                <div class="clear"></div>
                <textarea name="mensagem" cols="30" rows="10"></textarea>
                <button type="submit" class="btn">Enviar</button>
            </form>
            <div class="endereco">
                <p class="rua">Rua das aventuras, 9650</p>
                <p class="bairro">Jardin das Amelias</p>
                <p class="cidade">Bolotas | São Paulo</p>
            </div>
        </div>
        <div class="maps">
            <div class="mapouter">
                <div class="gmap_canvas">
                    <iframe width="100%" height="100%" id="gmap_canvas" src="https://maps.google.com/maps?q=2880%20Broadway,%20New%20York&t=&z=13&ie=UTF8&iwloc=&output=embed" frameborder="0" scrolling="no" marginheight="0" marginwidth="0"></iframe>
                </div>
            </div>
        </div>
        <div class="clear"></div>
    </section>
</template>

<script>
export default {
    name : "Contato",
    methods: {
        submit(e){
            e.preventDefault();
        }
    }
}
</script>

<style scoped>
section{
    width: 930px;
    margin: 0 auto;
    margin-bottom: 30px;
}
.form{
    max-width: 600px;
    margin: auto;
    float: left;
}
.maps{
    float:right;
    height: 450px;
}
.form .left{
    float: left;
}
.form .right{
    float: right;
}
.form input{
    width: 260px;
    padding: 5px 15px;
    border: 1px solid #2c3e50;
}
.form input:focus{
    outline: none;
    border: 1px solid #41b883;
}
.form textarea{
    margin-top: 20px;
    width: 594px;
    border: 1px solid #2c3e50;
    resize: none;
}
.form textarea:focus{
    outline: none;
    border: 1px solid #41b883;
}
.form button{
    margin: 10px 0px;
    width: 290px;
    padding: 10px 15px;
    border: none;
    font-size: 20px;
    color: #41b883;
    background: #2c3e50;
}
.form button:hover{
    cursor: pointer;
    background: #41b883;
    color: #2c3e50;
}
.form button:focus{
    outline: none;
}
.form .endereco{
    margin-top: 50px;
    font-size: 15px;
    font-style: italic;
}
.form .endereco p{
    margin: 9px 0px;
}
.mapouter{position:relative;text-align:right;height:100%;width:100%;}
.gmap_canvas {overflow:hidden;background:none!important;height:100%;width:100%;}
</style>