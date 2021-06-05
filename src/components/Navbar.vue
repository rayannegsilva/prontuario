<template>
  <b-container fluid class="main">
    <!-- NAV BAR -->
      <b-navbar class="navbar-div" type="light">
         <b-navbar-brand class="nav-brand">
           <b-img id="nav-brand-img" :src="require('../assets/LogoSipetiPreta.svg')" style="width: 100px"></b-img>
         </b-navbar-brand>

         <div>
          <!-- <b-icon-list class="show-menu nav-toggle"></b-icon-list> -->
         </div>
      </b-navbar>

    <!-- MENU LATERAL -->
  <div id="menu" class="menu-lateral">
    <div class="menu-cont">
      <div>
        <b-link class="title link" to="/login">
          <b-icon class="menu-logo icons-menu" icon="plus-circle"></b-icon>
          <span class="menu-title"> SiPETI</span>
         </b-link>

          <div class="menu-list">
            <div class="menu-itens">
        
              <h3 class="subtitle">Menu</h3>

              <b-link class="link">
                <b-icon class="icons-menu" icon="house-door"></b-icon>
                <span class="menu-name">Home</span>
              </b-link>

              <b-link class="link">
                <b-icon class="icons-menu" icon="person-circle"></b-icon>
                <span class="menu-name">Perfil</span>
              </b-link>

              <b-link class="link">
                <b-icon class="icons-menu" icon="clipboard-data"></b-icon>
                <span class="menu-name">Gráficos</span>
              </b-link>
            </div>

            <div class="menu-itens">
              <h3 class="subtitle"> Atendimento </h3>

              <b-link class="link">
                <b-icon class="icons-menu" icon="person-plus"></b-icon>
                <span class="menu-name">Atendimento</span>
              </b-link>

               <b-link class="link">
                <b-icon class="icons-menu" icon="file-person"></b-icon>
                <span class="menu-name">Pacientes</span>
              </b-link>

            </div>
          </div>

      </div>

      <b-link class="link menu-logout">
        <b-icon class="icons-menu" icon="box-arrow-left"></b-icon>
        <span class="menu-name">Sair</span>
      </b-link>

    </div>
  </div>

  <b-container fluid style="padding-left:6rem; padding-top: 1.5rem">
    oi
  </b-container>

  </b-container>
</template>

<script>
    
   /* const showMenu = (navToggle, menuId) =>{
    const toggleBtn = document.getElementById(headerToggle),
    nav = document.getElementById(menuId)

     if(navToggle && menuId){
        toggleBtn.addEventListener('click', ()=>{
            // We add the show-menu class to the div tag with the nav__menu class
            nav.classList.toggle('show-menu')
            // change icon
            toggleBtn.classList.toggle('x')
        })
    }
}

showMenu('nav-toggle','men')*/

export default {
 

}
</script>

<style scoped>
*, ::before, ::after {
  box-sizing: border-box;
}

/*NAVBAR */
.navbar-div{
  background-color: #F9F6FD;
  box-shadow: 0 1px 0 rgba(22, 8, 43, 0.1);
}
.navbar-brand{
margin-left: 80px;
}
.nav-toggle{
   font-size: 1.2rem;
   cursor: pointer;
   color: #101010;
}

/*MENU LATERAL*/
.menu-lateral{
  position: fixed;
  top: 0;
  background-color: #F9F6FD;
 /* left: -100%; */
  height: 100vh;
  z-index: 100;
  padding: 1rem 1rem 0;
  transition: .4s;
  box-shadow: 1px 0 0 rgba(22, 8, 43, 0.1);
}
.menu-cont{
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding-bottom: 3rem;
  overflow: auto;
}
.menu-cont::-webkit-scrollbar {
  display: none;
}
.title{
  text-decoration: none;
  margin-bottom: 2.5rem;
}
.menu-logo{
color: #101010; 
font-size: 1.2rem;
margin-right: 0rem;
text-decoration: none;
cursor: pointer;
}
.menu-title{
  font-weight: 600;
  color: #101010;
  font-size: 1.4rem;
}
.menu-list, .menu-itens{
  display: grid;
}
.menu-list{
  row-gap: 2.5rem;
}
.menu-itens{
  row-gap: 1.5rem;
}
.subtitle{
  font-size: 1rem;
  text-transform: uppercase;
  letter-spacing: .1rem;
  font-weight: 600;
  color: #c4bcce;
}
.icons-menu{
  margin-right: .5rem;
  font-size: 1.2rem;
}
.menu-name{
  font-size: .938rem;
  font-weight: 500;
  white-space: nowrap;
}
.link {
  display: flex;
  align-items: center;
  color: #101010;
  text-decoration: none;
}
.link:hover {
  color: #C6EEC5;
}

.active {
  color: red;
}
@media screen and (min-width: 768px) {
  .menu-lateral{
    left: 0;
    padding: 1.2rem 1.5rem 0;
    width: 68px; /* Reduced navbar */
}
.icons-menu{
    font-size: 1.2rem;
}
.menu-title, 
.menu-name, 
.subtitle {
    opacity: 0;
    transition: .3s;
  }

.menu-lateral:hover {
    width: 219px;
  }

/* Visible elements */
  .menu-lateral:hover .menu-title {
    opacity: 1;
  }
  .menu-lateral:hover .subtitle {
    opacity: 1;
  }
  .menu-lateral:hover .menu-name {
    opacity: 1;
  }
  /*.menu-lateral:hoverr .nav__dropdown-icon {
    opacity: 1;
  }*/

}
</style>
