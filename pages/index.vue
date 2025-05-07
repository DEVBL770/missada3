<template>
    <div
      class="min-h-screen bg-cover bg-center px-4 py-8"
      style="background-image: url('https://images.unsplash.com/photo-1600891964599-f61ba0e24092?auto=format&fit=crop&w=1950&q=80')"
    >
      <div class="backdrop-blur-sm bg-black/70 rounded-xl max-w-4xl mx-auto p-6 shadow-xl">
        <Header />
        <MenuSection title="Pizzas" :items="menu.pizzas" />
        <MenuSection title="Pâtes" :items="menu.pates" />
        <MenuSection title="Desserts" :items="menu.desserts" />
        <MenuSection title="Boissons" :items="menu.boissons" />
        <Footer />
      </div>
    </div>
  </template>
  
  <script setup>
  import Header from '@/components/Header.vue'
  import MenuSection from '@/components/MenuSection.vue'
  import Footer from '@/components/Footer.vue'
  
  const menu = {
    pizzas: [
      {
        name: 'Margherita',
        description: 'Tomate, mozzarella, basilic frais',
        price: 10,
        image: 'https://images.unsplash.com/photo-1601924579778-d74302c2732b?w=400&q=80'
      },
      {
        name: 'Reine',
        description: 'Tomate, jambon, champignons, mozzarella',
        price: 12,
        image: 'https://images.unsplash.com/photo-1613145991414-20c6ee4fa2c1?w=400&q=80'
      },
      {
        name: 'Quattro Formaggi',
        description: 'Gorgonzola, mozzarella, parmesan, chèvre',
        price: 13,
        image: 'https://images.unsplash.com/photo-1571091718767-18b5b1457add?w=400&q=80'
      },
      {
        name: 'Calzone',
        description: 'Tomate, mozzarella, jambon, œuf',
        price: 12,
        image: 'https://images.unsplash.com/photo-1601924857980-c9e6f5d11a56?w=400&q=80'
      },
    ],
    pates: [
      {
        name: 'Spaghetti alla Carbonara',
        description: 'Lardons, œuf, parmesan, poivre',
        price: 11,
        image: 'https://images.unsplash.com/photo-1589308078050-972054e3a25d?w=400&q=80'
      },
      {
        name: 'Tagliatelle al Pesto',
        description: 'Pesto maison, pignons de pin, parmesan',
        price: 12,
        image: 'https://images.unsplash.com/photo-1603133872878-684f208fb84f?w=400&q=80'
      },
      {
        name: 'Lasagnes Bolognaises',
        description: 'Viande hachée, sauce tomate, béchamel',
        price: 13,
        image: 'https://images.unsplash.com/photo-1589187155471-08e60f63d1d9?w=400&q=80'
      },
    ],
    desserts: [
      {
        name: 'Tiramisu',
        description: 'Recette traditionnelle au café',
        price: 6,
        image: 'https://images.unsplash.com/photo-1608219959573-93dbee7d4106?w=400&q=80'
      },
      {
        name: 'Panna Cotta',
        description: 'Coulis de fruits rouges',
        price: 5,
        image: 'https://images.unsplash.com/photo-1642393177401-5d0b9d34b61e?w=400&q=80'
      },
      {
        name: 'Gelato maison',
        description: '3 boules au choix',
        price: 5.5,
        image: 'https://images.unsplash.com/photo-1606731481200-08b6cd5b2c08?w=400&q=80'
      },
    ],
    boissons: [
      {
        name: 'Chianti DOCG',
        description: 'Verre de vin rouge italien',
        price: 6,
        image: 'https://images.unsplash.com/photo-1588866298361-7165e542a344?w=400&q=80'
      },
      {
        name: 'Eau pétillante',
        description: 'San Pellegrino 50cl',
        price: 3,
        image: 'https://images.unsplash.com/photo-1615751072497-e7b9d20bd40f?w=400&q=80'
      },
      {
        name: 'Soda',
        description: 'Coca, Fanta, Sprite...',
        price: 2.5,
        image: 'https://images.unsplash.com/photo-1626963187221-29fc2d4f2c8e?w=400&q=80'
      },
      {
        name: 'Café espresso',
        description: 'Pur arabica italien',
        price: 2,
        image: 'https://images.unsplash.com/photo-1572441710530-969d7a5d0b01?w=400&q=80'
      },
    ]
  }
  </script>
  