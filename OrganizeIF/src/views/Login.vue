<template>
  <ion-content>
    <div class="background-container">
      <ion-page class="page-login">
        <form action="" class="form-login">
          <ion-card>
            <ion-item>
              <h3>LOGIN</h3>
            </ion-item>
            <ion-item>
              <ion-label position="floating">Email</ion-label>
              <ion-input required v-bind="field" type="text" name="taskField"
                        placeholder="Insira o seu email"></ion-input>
            </ion-item>
            <ion-item>
              <ion-label position="floating">Senha</ion-label>
              <ion-input required v-bind="field" type="password" name="taskField"
                        placeholder="Insira sua senha"></ion-input>
            </ion-item>

            <ion-item>
              <ion-button type="submit" size="small" shape="round">
                Entrar
                <ion-icon slot="end" :icon="logIn"></ion-icon>
              </ion-button>
              <ion-button @click="$router.push('/signup')" type="submit" size="small" shape="round">
                Não possuo login
                
                <ion-icon slot="end" :icon="logIn"></ion-icon>
              </ion-button>
            </ion-item>

            
          </ion-card>
        </form>
      </ion-page>
    </div>
  </ion-content>
</template>

<script>
export default {
  name: 'login',
  data: function(){
    return {};
  }
};
</script>

<style scoped>

</style>