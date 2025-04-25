<template>
  <header class="header bg-main">
    <div class="header-group">
      <div class="flex justify-between items-center py-10">
        <div class="w-28 lg:w-36">
          <img
            class="w-full"
            src="../../src/assets/img/logo_white 1.png"
            alt="Logo"
          />
        </div>
        <div class="flex">
          <button
            class="px-6 py-2 font-bold rounded-full text-white focus:outline-none cursor-pointer"
          >
            Entrar
          </button>
          <button
            class="px-6 py-2 font-bold bg-white rounded-full text-main focus:outline-none cursor-pointer"
          >
            Crie um conta
          </button>
        </div>
      </div>
      <div class="flex flex-col mt-28">
        <h1 class="text-4xl lg:text-5xl font-bold text-white text-center">
          Tenha um feedback.<br />
          E faça seu cleinte mais <br class="hidden lg:inline-block" />
          feliz.
        </h1>
        <p class="text-lg font-medium text-white">
          Receba ideias, reclamações e feedbacks com um
          <br class="hidden lg:inline-block" />
          simples widget na página.
        </p>
        <div>
          <button
            class="px-6 py-2 font-bold bg-white rounded-full text-main focus:outline-none cursor-pointer mt-10"
          >
            Crie uma conta grátis
          </button>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {};
</script>

<style lang="postcss" scoped>
.header {
  @apply bg-main w-full flex justify-center;
  height: 700px;
}
.header-group {
  @apply flex flex-col justify-center w-4/5 max-w-6xl m-auto;
}
@media (min-width: 640px) {
  .header-group {
    background-image: url("../../src/assets/img/png-transparent-several-blue-balloons-balloon-navy-blue-blue-balloon-blue-simple-greeting-card 2.png");
    background-size: 682px 682px;
    background-position: 90% 100%;
    background-repeat: no-repeat;
    display: block;
    width: 100%;
  }
}
</style>
