<template>
  <div>
    <b-navbar>
      <template #brand>
        <b-navbar-item tag="router-link" :to="{ path: '/' }">
          <p class="titulo-inicial"><i>Plan!</i></p>
        </b-navbar-item>
      </template>
      <template #start> </template>
      <template #end>
        <b-navbar-item tag="div">
          <div class="buttons">
            <b-button
              type="is-primary is-outlined is-rounded"
              tag="nuxt-link"
              to="/cadastro/cadastrar"
            >
              <strong>Cadastre-se</strong></b-button
            >
            <b-button
              type="is-primary is-outlined is-rounded"
              tag="nuxt-link"
              to="/cadastro/entrar"
              >Entrar</b-button
            >
            <b-button
              type="is-primary is-outlined is-rounded"
              tag="nuxt-link"
              to="/task/task"
              >Task</b-button
            >
          </div>
        </b-navbar-item>
      </template>
    </b-navbar>
    <Nuxt />
  </div>
</template>

<script>
export default {}
</script>
<style scoped>
p {
  color: #023e8a;
}
.is-link {
  color: #023e8a;
}
</style>