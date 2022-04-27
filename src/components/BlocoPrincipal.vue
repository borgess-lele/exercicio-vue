<script>
import NovoBloco from "./NovoBloco.vue";
export default {
  components: { NovoBloco },
  data() {
    return {
      alunos: ["heloisa", "eduardo"],
    };
  },
};
</script>
<template>
  <main id="content">
    <NovoBloco class="Bloco 1" :nomes="['Heloisa', 'Eduardo']" />
    <NovoBloco class="alerta" :nomes="['Eduardo', 'wedley']" />
    <NovoBloco class="novo" :nomes="['Eduardo', 'Wedley']" />
    <NovoBloco class="urgente" :nomes="['Eduardo', 'Wedley']" />
    <NovoBloco class="nome" :nomes="['alunos']" />
  </main>
</template>
<style></style>
