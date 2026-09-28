<script setup>
import ProductCard from '../components/ProductCard.vue'
 
const daftarProduk = [
  { id: 1, nama: 'Como', harga: 900000, gambar: 
'https://shop.comofootball.com/cdn/shop/files/1_136c676b-945d-4f51-b4f6-abf3e9b9e7fd.jpg?v=1787067717&width=2000' },
  { id: 2, nama: 'Como', harga: 300000, gambar: 
'https://shop.comofootball.com/cdn/shop/files/StickerJacketfront.jpg?v=1787843437&width=1100' },
  { id: 3, nama: 'Como', harga: 120000, gambar: 
'https://shop.comofootball.com/cdn/shop/files/1_4_ab31d12d-7826-4da5-b3e6-c5119b8ac93c.jpg?v=1784910164&width=2000' },
 { id: 4, nama: 'Como', harga: 1000000, gambar: 
'https://shop.comofootball.com/cdn/shop/files/Image1_4f3b4133-746e-4bd6-ab02-28aa378ffbf3.jpg?v=1775838281&width=1100' },
 { id: 5, nama: 'Como', harga: 200000, gambar: 
'https://shop.comofootball.com/cdn/shop/files/1_136c676b-945d-4f51-b4f6-abf3e9b9e7fd.jpg?v=1787067717&width=1100' },
 { id: 6, nama: 'Como', harga: 1500000, gambar: 
'https://shop.comofootball.com/cdn/shop/files/Retro_9_Longsleeve_Como_Logo_Front.jpg?v=1774958410&width=2000'},
{id: 7, nama: `Como`, harga: 1300000, gambar :
`https://shop.comofootball.com/cdn/shop/files/1_5e134139-14fd-4950-898c-ea7c84ebfc9b.jpg?v=1787067117&width=2000` },
{id: 8, nama: `Como`, harga: 1500000, gambar :
`https://shop.comofootball.com/cdn/shop/files/Retro7JumperBlueWhiteCollar_Front_1.jpg?v=1773314866&width=2000`},
]
</script>
 




<template>
  <main>
    <h1><b>PRODUK KAMI</b></h1>
    <div class="grid">
      <ProductCard
        v-for="produk in daftarProduk"
        :key="produk.id"
        :nama="produk.nama"
        :harga="produk.harga"
        :gambar="produk.gambar"
      />
    </div>
  </main>
</template>

<style scoped>
.grid {
  display: flex;
  gap: 16px;
  align-items: stretch;
  flex-wrap: wrap;
}
.btn-grad {
  background-image: linear-gradient(to right, #0f358b 0%, #182848 51%, #030303 100%);
  }

  .btn-grad  {
    margin: 10px;
    padding: 15px 45px;
    text-align: center;
    text-transform: uppercase;
    transition: 0.5s;
    background-size: 200% auto;
    color: white;
    box-shadow: 0 0 20px #eee;
    border-radius: 10px;
    display: block;
    outline: none;
    border: none;
  }

  .btn-grad:hover {
    background-position: right center;
    color: #fff;
    text-decoration: none;
  }
</style>