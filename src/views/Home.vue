<template>
  <div class="home">
    <section id="banner">
      <div class="banner">
        <img src="https://via.placeholder.com/1350x500" alt="">
        <div class="description">
          <p class="title">Loren Ipsulum</p>
          <p class="text">There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable.</p>
        </div>
      </div>
    </section>
    <section id="services">
      <p class="section-title">Nossos Serviços</p>
      <p class="section-subtitle">Veja os serviços fornecidos por nossa companhia.</p>
      <div class="box-section">
        <div class="box">
          <div class="icon"></div>
          <p class="title">Loren Ipsulum</p>
          <p class="description">There are many variations of passages of Lorem Ipsum available.</p>
        </div>
        <div class="box">
          <div class="icon"></div>
          <p class="title">Loren Ipsulum</p>
          <p class="description">There are many variations of passages of Lorem Ipsum available.</p>
        </div>
        <div class="box">
          <div class="icon"></div>
          <p class="title">Loren Ipsulum</p>
          <p class="description">There are many variations of passages of Lorem Ipsum available.</p>
        </div>
        <div class="clear"></div>
      </div>
    </section>
    <section id="applications">
      <div class="apps">
        <div class="circles">
          <div class="circle light"></div>
          <div class="circle dark"></div>
          <div class="clear"></div>
        </div>
        <div class="statistics">
          <p class="info">
            <spam class="number">42</spam><br>
            <spam class="text">Colaboradores</spam>
          </p>
          <p class="info">
            <spam class="number">20</spam><br>
            <spam class="text">Aplicações Desenvolvidas</spam>
          </p>
          <p class="info">
            <spam class="number">7</spam><br>
            <spam class="text">Clientes Satisfeitos</spam>
          </p>
        </div>
      </div>
      <div class="clear"></div>
    </section>
  </div>
</template>

<script>

export default {
  name: 'Home'
}
</script>

<style scoped>
.banner{
  width: 100%;
}
.banner img{
  width: 100%;
}
.banner .img{
  background: url(https://via.placeholder.com/1350x500);
  width: 100%;
  height: 500px;
}
.banner .description{
  z-index: 9999;
  position: absolute;
  margin-top: -300px;
  padding: 50px;
  width: 500px;
  background: rgba(0, 0, 0, 0.15);
}
.banner .description .title{
  font-size: 63px;
  margin: 0px 0px 20px 0px;
}
.banner .description .text{
  font-size: 20px;
  margin: 0;
}
.box-section{
  max-width: 960px;
  margin: 63px auto auto auto;
  padding-bottom: 70px;
}
.box-section .box{
  float: left;
  height: auto;
  max-width: 250px;
  border: 1px solid #35495e;
  padding: 10px;
  margin: 10px 23px;
}
.box-section .box .title{
  font-size: 30px;
  margin: 15px 0px;
  text-align: center;
}
.box-section .box .description{
  text-align: center;
}
.box-section .box .icon{
  height: 100px;
  width: 100px;
  border-radius: 50%;
  background: #41b883;
  margin: auto
}
.box-section .box:hover{
  background: #41b883;
  border: 1px solid white;
  color: white;
}
.box-section .box:hover .icon{
  background: #35495e;
}
.apps{
  max-width: 705px;
  margin: auto auto 60px auto;
  height: 300px;
}
.circles{
  float: left;
}
.circles .circle{
  height: 300px;
  width: 300px;
  border-radius: 50%;
  float:left;
}
.circles .light{
  background: #6b96c2;
  box-shadow: 0 0 5px #6b96c2;
}
.circles .dark{
  background: #2c3e50;
  box-shadow: 0 0 5px #2c3e50;
  z-index: 10;
  margin-left: -250px;
}
.statistics{
  float: left;  
}
.statistics .info{
  margin: 25px 30px;
}
.statistics .info .number{
  color: #6b96c2;
  font-size: 35px;
}
.statistics .info .text{
  color: #2c3e50;
  font-size: 25px;
}
</style>
