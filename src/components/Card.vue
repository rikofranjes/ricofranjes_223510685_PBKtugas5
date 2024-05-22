<template>
    <div class="q-pa-md">
      <div class="grid-wrapper q-gutter-md">
        <q-card v-for="(card, index) in cards" :key="index" class="my-card">
          <img :src="card.img" class="card-img">
          <q-card-section>
            <div class="text-h6">{{ card.title }}</div>
            <div class="text-subtitle2">{{ card.harga }}</div>
          </q-card-section>
          <q-card-section class="q-pt-none">
            {{ card.description }}
          </q-card-section>
        </q-card>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    setup() {
      return {
        cards: [
          {
            img: "https://img.freepik.com/premium-photo/row-fashionable-polo-tshirts-man-wooden-hanger-rack-clothing-boutique-retail-shop_326694-48415.jpg?size=626&ext=jpg&ga=GA1.2.1231175041.1716021742&semt=ais_user",
            title: "Shirt superme",
            harga: "Rp 120.000",
            description: "lorem ipsum dolor sit amet"
          },
          {
            img: "https://img.freepik.com/premium-photo/row-fashionable-polo-tshirts-man-wooden-hanger-rack-clothing-boutique-retail-shop_326694-47545.jpg?size=626&ext=jpg&ga=GA1.1.1231175041.1716021742&semt=ais_user",
            title: "Baju Polos",
            harga: "Rp 150.000",
            description: "Baju desain polos"
          },
          {
            img: "https://img.freepik.com/free-photo/apparel-embossed-logo-mockup_23-2149779520.jpg?t=st=1716034784~exp=1716038384~hmac=ce01bc80835975a525adb372b334b372bd4ef903f26907353f9e12cb0138bb25&w=740",
            title: "Hoodie Shirt",
            harga: "Rp 200.000",
            description: "Hoodie desain polos"
          },
          {
            img: "https://img.freepik.com/free-photo/happy-couple-stylish-hoodies-winter-outdoor-shoot_53876-105545.jpg?t=st=1716034910~exp=1716038510~hmac=7d206cb1e011a059fedee3e31f763e099530946467c6864e1af4fad8a2a67ab2&w=740",
            title: "Hoodie",
            harga: "Rp 500.000",
            description: "Hoodie stylish outdoor"
          },
          {
            img: "https://img.freepik.com/free-photo/sport-jacket-clothing_1203-2534.jpg?t=st=1716034975~exp=1716038575~hmac=31b0e6296b5e448d91173f51eb0dc2065e34ecaf745469f1b117c2e22557e0a4&w=740",
            title: "Jacket Clothing",
            harga: "Rp 500.000",
            description: "jacket Sport"
          },
          {
            img: "https://img.freepik.com/free-photo/business-casual-shirt-white-closeup-outdoor-photoshoot_53876-119744.jpg?t=st=1716035116~exp=1716038716~hmac=277326106022541123ee15b77eec55a256edfcd57c0dfc38a614c36c2754af09&w=740",
            title: "Kemeja",
            harga: "Rp 650.000",
            description: "Kemeja Putih Polos"
          },
          {
            img: "https://img.freepik.com/free-photo/bff-printed-red-hoodie_53876-105408.jpg?t=st=1716035185~exp=1716038785~hmac=26bdfd5a62c2a1eb2720cf9c2211f7f3ec0c88ed269e2f9fee2424184ee32660&w=740",
            title: "Jacket Hoodie",
            harga: "Rp 450.000",
            description: "jacket hoodie Bertulisan BFF"
          },
          {
            img: "https://img.freepik.com/free-psd/hanes-adult-tagless-longsleeve-tee-mockup_126278-60.jpg?t=st=1716035369~exp=1716038969~hmac=d68d1ed9c023b7893a2296d83eef4e62638c0919b70c9cc6ca6c9e4f7f6f3fe1&w=740",
            title: "Long sleeve shirt",
            harga: "Rp 200.000",
            description: "long sleeve shirt untuk orang dewasa "
          }
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  .grid-wrapper {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 16px;
  }
  
  .my-card {
    width: 100%;
    max-width: 100%;
    background-image: linear-gradient(163deg, #c9f5f6 10%, #F6EEC9 100%);
    border-radius: 5px;
    transition: all .3s;
    cursor: pointer;
  }
  
  .card-img {
    width: 100%;
    height: auto;
  }
  
  .my-card:hover {
    transform: scale(0.98);
  }
  
  @media (max-width: 600px) {
    .grid-wrapper {
      grid-template-columns: 1fr;
    }
  
    .my-card {
      margin-bottom: 16px;
    }
  }
  </style>