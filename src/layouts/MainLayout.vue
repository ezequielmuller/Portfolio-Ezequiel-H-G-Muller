<template>
  <q-layout view="hHh lpR fFf">
    <q-header class="transparent-header">
      <q-toolbar class="q-gutter-sm items-center justify-between q-col-gutter-sm">
        <div class="row items-center q-gutter-sm">
          <q-btn flat dense round icon="menu" @click="gerenciarMenu" class="q-mr-sm" />
          <q-icon name="code" size="md" />
          <q-toolbar-title class="text-bold">Ezequiel H. G. Muller - Developer</q-toolbar-title>
        </div>
      </q-toolbar>
      <q-separator color="#EAEBFA" size="1px" inset class="q-mt-sm" />
    </q-header>

    <!-- Menu -->
    <q-drawer v-model="menu" side="left" bordered show-if-above>
      <q-list padding>
        <q-item clickable v-ripple>
          <q-item-section>Me Conheça</q-item-section>
        </q-item>
        <q-item clickable v-ripple>
          <q-item-section>Habilidades</q-item-section>
        </q-item>
        <q-item clickable v-ripple>
          <q-item-section>Redes Sociais</q-item-section>
        </q-item>
        <q-item clickable v-ripple>
          <q-item-section>Projetos</q-item-section>
        </q-item>
        <q-item clickable v-ripple>
          <q-item-section>
            <q-btn label="Fale Comigo" no-caps color="primary" class="full-width" />
          </q-item-section>
        </q-item>
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer>
      <div class="row q-col-gutter-md">
        <div class="col-12 flex justify-end items-center">
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
      <div id="ultima-div" class="row q-col-gutter-md justify-center items-center text-center">
        <div class="col-md-4 col-sm-4 col-xs-12 flex justify-center items-center">
          <q-icon name="code" size="sm" /> Ezequiel H. G. Muller - Developer
        </div>
        <div class="col-md-4 col-sm-4 col-xs-12 flex justify-center items-center">
          <q-icon name="copyright" /> 2025 Ezequiel Muller - Todos os direitos reservados
        </div>
      </div>
    </q-footer>
  </q-layout>
</template>

<script lang="ts" setup>
import { ref } from 'vue'
const menu = ref(false)


const gerenciarMenu = () => {
  menu.value = !menu.value
}

</script>
