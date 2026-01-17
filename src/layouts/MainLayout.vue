<template>
  <q-layout view="lHh Lpr lFf" class="bg-black text-white">
    <q-header class="bg-transparent text-white q-py-sm" style="backdrop-filter: blur(10px)">
      <q-toolbar>
        <q-toolbar-title class="text-weight-bold text-h5">
          <span class="text-red">C</span>ustomer<span class="text-red">M</span>anager
        </q-toolbar-title>

        <div class="q-gutter-md gt-sm">
          <q-btn flat no-caps label="Home" to="/" />
          <q-btn flat no-caps label="Features" />
          <q-btn flat no-caps label="Pricing" />
          <q-btn flat no-caps label="About" />
          <q-btn
            unelevated
            color="primary"
            label="Get Started"
            no-caps
            class="q-px-lg"
            @click="loginOpen = true"
          />
        </div>

        <q-btn flat dense round icon="menu" class="lt-md" />
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

    <!-- Login Dialog -->
    <q-dialog v-model="loginOpen">
      <q-card class="glass-card text-white" style="width: 400px; max-width: 90vw">
        <q-card-section class="q-pt-lg q-pb-none text-center">
          <div class="text-h5 text-weight-bold text-gradient q-mb-sm">CustomerManager</div>
          <div class="text-subtitle1 text-grey-4">Sign In</div>
        </q-card-section>

        <q-card-section class="q-pa-lg">
          <q-form class="q-gutter-md">
            <q-input filled dark v-model="username" label="Username" color="red" bg-color="grey-10">
              <template v-slot:prepend>
                <q-icon name="person" color="red" />
              </template>
            </q-input>

            <q-input
              filled
              dark
              v-model="password"
              label="Password"
              type="password"
              color="red"
              bg-color="grey-10"
            >
              <template v-slot:prepend>
                <q-icon name="lock" color="red" />
              </template>
            </q-input>

            <div class="q-mt-lg">
              <q-btn
                unelevated
                color="primary"
                size="lg"
                class="full-width"
                label="Sign In"
                no-caps
                @click="loginOpen = false"
              />
            </div>
          </q-form>
        </q-card-section>
      </q-card>
    </q-dialog>
  </q-layout>
</template>

<script setup>
import { ref } from 'vue'

const loginOpen = ref(false)
const username = ref('')
const password = ref('')
</script>

<style scoped>
.glass-card {
  background: rgba(43, 43, 43, 0.8);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.1);
}
</style>
