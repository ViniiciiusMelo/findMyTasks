<template>
  <section class="section has-background-primary tamanho-login">
    <div class="container">
      <div class="columns is-mobile is-centered">
        <div class="column is-4">
          <div class="box">
            <div class="columns is-mobile is-centered">
              <div class="column is-7">
                <b-image
                  :src="require('@/assets/images/logoPLan1.png')"
                  alt="Plan logo"
                ></b-image>
              </div>
            </div>
            <b-field label="E-mail" label-position="inside">
              <b-input
                placeholder="joao.barro@gmail.com"
                type="email"
                maxlength="60"
                icon="envelope"
              ></b-input>
            </b-field>
            <b-field label="Senha" label-position="inside">
              <b-input type="password" maxlength="30" icon="key"></b-input>
            </b-field>
            <div class="block has-text-centered">
              <b-button type="is-primary is-outlined" expanded icon-right="user"
                ><strong>Entrar</strong></b-button
              >
            </div>
            <div class="block has-text-centered">
              <p>
                Não possui uma conta?
                <NuxtLink to="/cadastro/cadastrar">Clique aqui</NuxtLink> e
                cadastre-se!
              </p>
            </div>
            <div class="block has-text-centered">
              <NuxtLink to="/">Voltar ao início</NuxtLink>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  layout: 'cadastro/cadastroPrincipal',
  data() {
    return {}
  },
}
</script>
<style>
.tamanho-login {
  min-height: 100vh;
}
</style>