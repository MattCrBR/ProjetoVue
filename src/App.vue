<template>
  <div class="page">
    <header class="header">
      <h1>Lume3D</h1>
      <p>Plataforma de produtos impressos em 3D</p>
    </header>
    <div class="products">
      <div class="card" v-for="product in products" :key="product.id">
        <div class="card-icon"></div>
        <h3>{{ product.name }}</h3>
        <p class="desc">{{ product.desc }}</p>
        <p class="price">{{ product.price }}</p>
        <button>Adicionar</button>
      </div>
    </div>
    <footer class="footer">
      Lume3D © 2025 — Todos os direitos reservados
    </footer>
  </div>
</template>

<script setup>
import './style.css'
const products = [
  { id: 1, name: 'Vaso para plantas', desc: 'Vaso com acabamento opaco preto', price: 'R$ 29,90' },
  { id: 2, name: 'Porta Canetas', desc: 'Porta Canetas em PLA preto', price: 'R$ 29,90' },
  { id: 3, name: 'Porta Palhetas', desc: 'Porta Palhetas impressa em PETG', price: 'R$ 19,90' },
]
</script>