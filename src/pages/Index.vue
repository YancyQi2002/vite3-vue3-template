<script setup lang="ts">
import HelloWorld from '@components/HelloWorld.vue'
import Footer from '@components/Footer/Footer.vue'
import BackTop from '@components/BackTop/BackTop.vue'
import * as tauriVer from '@/utils/tauriVer'
</script>

<template>
  <d-layout>
    <d-content>
      <div class="w-full h-full flex items-center justify-center py-12 px-4 sm:px-6 lg:px-8">
        <div class="max-w-md w-full h-full space-y-8">
          <div>
            <div class="flex">
              <img
                class="mx-auto h-12 w-auto" 
                src="https://tailwindui.com/img/logos/workflow-mark-indigo-600.svg"
                srcset="/tailwindcss.avif"
                loading="lazy"
                alt="tailwind"
                onerror="this.classList.add('error');"
              />
              <img
                class="mx-auto h-12 w-auto"
                src="/vite.svg"
                srcset="/vite.avif"
                loading="lazy"
                alt="vite"
                onerror="this.classList.add('error');"
              />
              <img
                class="mx-auto h-12 w-auto"
                src="@/assets/vue.svg"
                loading="lazy"
                alt="vue"
                onerror="this.classList.add('error');"
              />
            </div>
            <h2 class="text-3xl">
              Hello World!
            </h2>
          </div>
          <div>
            <HelloWorld msg="Vite 3 + Vue 3 TEMPLATE"/>
          </div>
        </div>
      </div>
    </d-content>
    <d-footer>
      <Footer />
    </d-footer>
    <BackTop />
  </d-layout>
</template>

<style scoped>
h2 {
  @apply m-6 text-center font-extrabold text-gray-900 select-none;
}
</style>