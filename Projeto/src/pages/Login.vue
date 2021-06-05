<template>
  <b-container fluid class="app">
   <!-- <b-container fluid class="circle"></b-container> -->
   <b-container fluid>
     <b-row>
       <b-col>
         <div>
          <b-img :src="require('../assets/IFSIMBOLO.png')" style="width: 30px; margin-top: 0.5rem; margin-left: 2.6rem"></b-img>
        </div>
         <div>
            <b-img :src="require('../assets/login1.svg')" style="width: 70%; margin-top: 4.5rem; margin-left: 2.5rem"></b-img>
         </div>
       </b-col>
       <b-col>
         <div>
            <b-img :src="require('../assets/LogoSipetiPreta.svg')" style="width: 40%; margin-top:6.8rem; margin-left: 12rem"></b-img>
         </div>
         <div class="form-div">
           <div class="form" style="margin-left: 60px;">
           <b-form  @submit="onSubmit" @reset="onReset" >
            <b-form-group  style="margin-top: 30px; max-width: 500px"
            label="Email de Acesso:"
            label-for="email_acesso"
            description="We'll never share your email with anyone else."
            >
              <b-form-input
              v-model="email"
              id="email_acesso" 
              type="email"
              placeholder="Digite seu email"
              />
            </b-form-group>
            <b-form-group style="margin-top: 10px; max-width: 500px"
             label="Senha:"
            label-for="senha"
            >
              <b-form-input
                id="senha"
                type="password"
              />
            </b-form-group>
           <div>
              <b-row style="">
              <b-col>
            <b-form-checkbox style=""
            v-model="lembrar"
            >Lembrar de mim</b-form-checkbox>
              </b-col>
              <b-col  style="text-align:right; margin-right: 78px" >
                Esqueci a senha
              </b-col>
            </b-row>
           </div>
          </b-form>
          </div>
         </div>
       </b-col>
     </b-row>
   </b-container>
  </b-container>
</template>

<script>
export default {
}
</script>

<style>
</style>