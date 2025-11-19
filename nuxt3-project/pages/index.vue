<template>
  <div class="min-h-screen bg-gradient-to-br from-blue-50 to-indigo-100 flex items-center justify-center p-6">
    <div class="max-w-4xl w-full">
      <div class="bg-white rounded-2xl shadow-2xl p-8 md:p-12">
        <h1 class="text-4xl md:text-5xl font-bold text-gray-800 mb-4 text-center">
          Selamat Datang di Nuxt 3 + Tailwind CSS
        </h1>
        <p class="text-lg text-gray-600 text-center mb-8">
          Project Anda sudah siap dengan Nuxt 3 dan Tailwind CSS!
        </p>
        
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
          <div class="bg-gradient-to-br from-blue-500 to-blue-600 rounded-xl p-6 text-white transform hover:scale-105 transition-transform duration-300">
            <div class="text-3xl mb-2">⚡</div>
            <h3 class="text-xl font-semibold mb-2">Nuxt 3</h3>
            <p class="text-blue-100">Framework Vue.js yang powerful untuk aplikasi modern</p>
          </div>
          
          <div class="bg-gradient-to-br from-indigo-500 to-indigo-600 rounded-xl p-6 text-white transform hover:scale-105 transition-transform duration-300">
            <div class="text-3xl mb-2">🎨</div>
            <h3 class="text-xl font-semibold mb-2">Tailwind CSS</h3>
            <p class="text-indigo-100">Utility-first CSS framework untuk styling yang cepat</p>
          </div>
          
          <div class="bg-gradient-to-br from-purple-500 to-purple-600 rounded-xl p-6 text-white transform hover:scale-105 transition-transform duration-300">
            <div class="text-3xl mb-2">🚀</div>
            <h3 class="text-xl font-semibold mb-2">Siap Pakai</h3>
            <p class="text-purple-100">Mulai coding sekarang juga!</p>
          </div>
        </div>

        <div class="bg-gray-50 rounded-xl p-6">
          <h2 class="text-2xl font-bold text-gray-800 mb-4">Langkah Selanjutnya:</h2>
          <ul class="space-y-3 text-gray-700">
            <li class="flex items-start">
              <span class="text-green-500 mr-2">✓</span>
              <span>Edit file <code class="bg-gray-200 px-2 py-1 rounded text-sm">pages/index.vue</code> untuk mengubah halaman ini</span>
            </li>
            <li class="flex items-start">
              <span class="text-green-500 mr-2">✓</span>
              <span>Buat halaman baru di folder <code class="bg-gray-200 px-2 py-1 rounded text-sm">pages/</code></span>
            </li>
            <li class="flex items-start">
              <span class="text-green-500 mr-2">✓</span>
              <span>Tambahkan komponen di folder <code class="bg-gray-200 px-2 py-1 rounded text-sm">components/</code></span>
            </li>
            <li class="flex items-start">
              <span class="text-green-500 mr-2">✓</span>
              <span>Gunakan Tailwind CSS classes untuk styling</span>
            </li>
          </ul>
        </div>

        <div class="mt-8 text-center">
          <button 
            @click="count++" 
            class="bg-gradient-to-r from-blue-500 to-indigo-600 text-white font-semibold px-8 py-3 rounded-lg shadow-lg hover:shadow-xl transform hover:-translate-y-1 transition-all duration-300"
          >
            Klik Saya: {{ count }}
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>
