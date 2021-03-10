<template>
  <div id="app">
    <header>
      <div id="contact-header">
        <div class="contatos-header">
          <a href="mailto:contato@empresa.com.br">contato@empresa.com.br</a>  |  (19) 99999-9999
        </div>
        <div class="midias-header">
          <div class="midia"><img src="./assets/facebook.svg" alt=""></div>
          <div class="midia"><img src="./assets/instagram.svg" alt=""></div>
          <div class="midia"><img src="./assets/linkedin.svg" alt=""></div>
        </div>
        <div class="clear"></div>
      </div>
      <div id="logo">
        <img src="./assets/logo.png" alt="">        
      </div>  
      <div id="nav-links">
        <router-link to="/">Home</router-link> |
        <router-link to="/sobre">Sobre</router-link> |
        <router-link to="/Contato">Contato</router-link>
      </div>
      <div class="clear"></div>
    </header>
    <router-view/>
    <footer>
      <div id="nav-links-footer">
        <ul>
          <li>
            <router-link class="nav-footer" to="/">Home</router-link>
          </li>
          <li>
            <router-link class="nav-footer" to="/sobre">Sobre</router-link>
          </li>
          <li>
            <router-link class="nav-footer" to="/Contato">Contato</router-link>
          </li>
        </ul>
      </div>
      <div class="contatos-footer">
        <p>
          <a href="mailto:contato@empresa.com.br">contato@empresa.com.br</a>
        </p>
        <p>
          (19) 99999-9999
        </p>  
        <div class="midias-footer">
          <div class="midia"><img src="./assets/facebook.svg" alt=""></div>
          <div class="midia"><img src="./assets/instagram.svg" alt=""></div>
          <div class="midia"><img src="./assets/linkedin.svg" alt=""></div>
        </div>
      </div>
      <div class="clear"></div>
    </footer>
  </div>
</template>

<style>
body{
  margin: 0;
  padding: 0;
}
header{
  background: #e4e4e4;
}
footer{
  padding: 5px 30px 40px;
  background: #3b3b3b;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

#nav-links {
  padding: 30px;
  float: right;
}

#nav-links a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
}

#nav-links a:hover{
  color: #577b9e;
}

#nav-links a.router-link-exact-active {
  color: #42b983;
}

#logo img{
  height: 80px;
}
#logo{
  float: left;
  padding: 5px 30px;
}
.clear{
  clear: both;
}
#contact-header{
  padding: 5px 30px;
  background: #2c3e50;
}
#nav-links-footer{
  float: left;
}
#nav-links-footer ul{
  padding: 0px;
}
#nav-links-footer ul li{
  list-style: none;
  margin-bottom: 3px;
}
#nav-links-footer ul li a{
  text-decoration: none;
  color: #42b983;
}
.contatos-header{
  float:left;
  color: white;
}
.contatos-footer{
  color: white;
  float:right;
  text-align: center;
}
.contatos-header a{
  text-decoration: none;
  color: white;
}
.contatos-footer a{
  text-decoration: none;
  color: #42b983;
}
.midias-header{
  float: right;
}
.midias-footer{
  float: right;
}
.midia{
  height: 20px;
  width: 20px;
  float: right;
  margin-left: 5px;
}
section .section-title{
  text-align: center;
  font-size: 50px;
  margin: 50px 0px 0px 0px;
  color: #41b883;
}
section .section-subtitle{
  text-align: center;
  color: #888787;
}
</style>
