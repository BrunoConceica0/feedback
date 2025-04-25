<template>
  <div>
    <custom-header @create-account="handleAccountCreate" @login="handleLogin" />
    <contact />
    <div class="flex justify-center py-10 bg-brand-gray">
      <p class="font-medium text-center text-gray-400">feedbacker © 2025</p>
    </div>
  </div>
</template>

<script>
import CustomHeader from "../Home/CustomHeader.vue";
import Contact from "../Home/Contact.vue";
import { onMounted } from "vue";

// Importando o onMounted do Vue para executar código após o componente ser montado
// import { useRouter } from "vue-router";
// Importando o useRouter do Vue Router para navegação

export default {
  components: { CustomHeader, Contact },
  setup() {
    // const router = useRouter();
    onMounted(() => {
      // Ao componentes montados, verifique se o token está presente no localStorage
      const token = localStorage.getItem("token");
      if (token) {
        // Se o token estiver presente, redirecione para a página de feedbacks, não precisa usar o $router.push somete router.push
        router.push({ name: "feedbacks" });
      }
    });
    // Define as functions para fazer login e criar conta
    function handleLogin() {}
    function handleAccountCreate() {}
    return {
      handleLogin,
      handleAccountCreate,
    };
  },
};
</script>

<style></style>
