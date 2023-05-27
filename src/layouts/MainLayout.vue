<template>
  <!-- <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="toggleLeftDrawer"
        />

        <q-toolbar-title> Quasar App </q-toolbar-title>

        <div>Quasar v{{ $q.version }}</div>
      </q-toolbar>
    </q-header>

    <q-drawer v-model="leftDrawerOpen" show-if-above bordered>
      <q-list>
        <q-item-label header> Essential Links </q-item-label>

        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout> -->

  <!-- Imagem de Abertura -->
  <div class="image">
    <!-- <h1>RotaFinanceira</h1> -->
    <div class="logo"></div>
  </div>
  <!-- Principal -->
  <div class="q-pa-lg text-center">
    <!-- Cabeçalho -->
    <div class="header">
      <h2 class="q-pa-none q-ma-none">
        Lorem ipsum dolor sit amet
      </h2>
      <h4 class="text-subtitle1 q-pa-noneq-pa-none q-ma-none">Lorem ipsum dolor sit amet</h4>
    </div>
    <!-- Menu -->
    <div class="nav-menu row">
      <button class="btn btn-secondary col">Registrar</button>
      <button class="btn btn-primary col">Entrar</button>
      <button class="btn btn-secondary col-12">Conectar com o Google</button>
    </div>
  </div>
</template>

<script>
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "MainLayout",
});
</script>

<style>
.image {
  display: flex;
  height: 523px;
  background-image: url("../../public/images/image62.png");
  background-repeat: no-repeat;
  background-size: cover;

  justify-content: center;
  align-items: center;
}

.header {
  padding-bottom: 24px;
}

.logo {
  display: block;
  width: 230px;
  height: 30px;
  background-image: url("../../public/images/logo.svg");
  background-repeat: no-repeat;
}

h2 {
  font-size: 24px;
  line-height: 22px;
  color: #293E2F;
}

h4 {
  color: #293E2F;
}

.nav {
  padding: 27px;
}

.nav-menu {
  gap: 16px;
}

.btn {
  border: none;
  align-items: center;
  padding: 16px 24px;

  height: 56px;

  border-radius: 60px;
}

.btn-primary {
  background: #8CE95F;
}

.btn-secondary {
  background: #E7F1E9;
}
</style>