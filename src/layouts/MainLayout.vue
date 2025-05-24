<template>
  <q-layout view="lHh Lpr lFf">
    <!-- Header -->
    <q-header class="transparent-header">
      <q-toolbar>
        <q-toolbar-title>
          <q-icon name="code" /> Ezequiel H. G. Muller
        </q-toolbar-title>
        <!-- @click="scrollToSection('redes')" -->
        <div class="row q-col-gutter-xs">
          <div class="col-xs-6 col-sm- col-md-auto">
            <q-btn flat label="Me Conheça" style="text-transform: none;" />
          </div>
          <div class="col-xs-6 col-sm-auto col-md-auto">
            <q-btn flat label="Habilidades" style="text-transform: none;" />
          </div>
          <div class="col-xs-6 col-sm-auto col-md-auto">
            <q-btn flat label="Redes Sociais" style="text-transform: none;" />
          </div>
          <div class="col-xs-6 col-sm-auto col-md-auto">
            <q-btn flat label="Projetos" style="text-transform: none;" />
          </div>
        </div>
      </q-toolbar>
      <q-separator color="grey-8" size="1px" inset />
    </q-header>

    <!-- Fundo de Vídeo
    <div class="video-background">
      <video autoplay muted loop id="background-video">
        <source src="src/assets/fundo.mp4" type="video/mp4" />
        Seu navegador não suporta a tag de vídeo.
      </video>
    </div> -->

    <!-- Conteúdo principal -->
    <q-page-container>
      <!--<div class="row q-col-gutter-md content-container">
        <div class="col-md-3 col-sm-12 image-container">
          <img src="src/assets/perfil.jpg" alt="Minha Foto" class="img-resized">
        </div>
        <div class="col-md-9 col-sm-12 text-container" style="color: #d0d0d0;">
          <p>
            Olá, meu nome é<span style="color:cornflowerblue;"> Ezequiel H. G. Müller</span>, sou de
            <span style="color:cornflowerblue;"> Marcelino Ramos/RS</span> e tenho 18 anos.

            Concluí em <span style="color:cornflowerblue;">2024</span> o Ensino Médio Integrado no
            <span style="color:cornflowerblue;">Instituto Federal de Educação, Ciência e Tecnologia do Rio Grande do Sul
              (IFRS) – Campus Erechim</span>,
            onde me formei como <span style="color:cornflowerblue;">Técnico em Informática</span>.
          </p>
          <p>
            Atualmente, estou cursando <span style="color:cornflowerblue;">Bacharelado em Ciência da Computação</span>
            na <em>Universidade
              Regional Integrada do Alto Uruguai e das Missões (URI) – Campus Erechim</em>.
          </p>
        </div>
      </div> -->
    </q-page-container>

    <!-- Parte inferior (Footer) -->
    <div class="row q-col-gutter-md">
      <div class="col-md-12 col-sm-12 col-xs-12" style="display: flex; justify-content: right; align-items: center;">
        <a href="https://github.com/ezequielmuller" target="_blank">
          <q-btn flat icon="fab fa-github" size="md" class="rounded-btn btn" />
        </a>
        <a href="https://linkedin.com/in/ezequielhgmuller" target="_blank">
          <q-btn flat icon="fab fa-linkedin" size="md" class="rounded-btn btn" />
        </a>
        <a href="https://www.instagram.com/ezequielmuller__/" target="_blank">
          <q-btn flat icon="fab fa-instagram" size="md" class="rounded-btn btn" />
        </a>
        <a href="https://www.instagram.com/ezequielmuller__/" target="_blank">
          <q-btn flat icon="fab fa-x-twitter" size="md" color="darkgrey" class="rounded-btn btn" />
        </a>
      </div>
    </div>
    <div id="ultima-div" class="row q-col-gutter-md"
      style="display: flex; justify-content: center; align-items: center; text-align: center;">
      <div class="col-md-4 col-sm-4 col-xs-12" style="display: flex; justify-content: center; align-items: center;">
        <q-icon name="code" size="sm" /> Ezequiel H. G. Muller
      </div>
      <div class="col-md-4 col-sm-4 col-xs-12" style="display: flex; justify-content: center; align-items: center;">
        <q-icon name="copyright" /> 2025 Ezequiel Muller - Todos os direitos reservados
      </div>
    </div>

  </q-layout>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'

export default defineComponent({
  setup() {
    return {
      codigo: ref('< />'),
      leftDrawerOpen: ref(false),
    }
  },
  methods: {
    toggleLeftDrawer() {
      this.leftDrawerOpen.value = !this.leftDrawerOpen.value
    }
  },
  async mounted() {

  }
})
</script>
