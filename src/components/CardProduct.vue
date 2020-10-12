<template>
  <div class="card shadow card-product">
    <div class="container">
      <img
        :src="'assets/images/' + product.gambar"
        alt="Card image cap"
        class="card-img-top"
        width="100"
        height="200"
      />
      <div class="card-body">
        <h5 class="card-title">{{ product.nama }}</h5>
        <p class="card-text">Harga : Rp. {{ product.harga }}</p>
        <router-link class="btn btn-success" :to=" 'foods/'+product.id"
          ><b-icon-cart></b-icon-cart> Pesan</router-link
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardProduct",
  props: ["product"],
};
</script>

<style>
</style>