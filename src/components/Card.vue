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
            img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTsZXd1Ri6m-L-3ldWo68QMLn-VUYYhjSAGUwR8hBr2bg&s",
            title: "Shirt superme",
            harga: "Rp 120.000",
            description: "lorem ipsum dolor sit amet"
          },
          {
            img: "https://thumbor.prod.raenabeauty.com/unsafe/filters:format(webp)/https://d1dnhxm90ph8r2.cloudfront.net/products/images/PBR001/ab0440da-a860-4b5b-a122-b9c0877deadd",
            title: "PINKBERRY",
            harga: "Rp 150.000",
            description: "TIPE 3"
          },
          {
            img: "https://dynamic.zacdn.com/Hw3EGagfJmMPKHpfAelzZckh-Ss=/filters:quality(70):format(webp)/https://static-id.zacdn.com/p/istana-boneka-3173-8274724-1.jpg",
            title: "romans wisH",
            harga: "Rp 200.000",
            description: "MODEL TERBARU"
          },
          {
            img: "https://id.ozcosmetics.com/prodimgs/202305/287086.jpg",
            title: "MY WAY",
            harga: "Rp 500.000",
            description: "GIORGIO ARMAN"
          },
          {
            img: "https://thefragranceshopinc.com/cdn/shop/products/image_6291effb-a45c-4170-9581-f8ce453dd616_1024x1024.jpg?v=1615160131",
            title: "SAUVAGE",
            harga: "Rp 500.000",
            description: "Parfum Sport"
          },
          {
            img: "https://img.id.my-best.com/product_images/ad31ee308c54179b0f6268c8247bdda6.jpeg?ixlib=rails-4.3.1&q=70&lossless=0&w=800&h=800&fit=clip&s=e4053645c7f36ede560da94c1ef7e560",
            title: "Mirror",
            harga: "Rp 650.000",
            description: "model terbaru"
          },
          {
            img: "https://down-id.img.susercontent.com/file/id-11134207-7r98q-lpj70axnm5svee",
            title: "EAJD",
            harga: "Rp 450.000",
            description: "Bertulisan BFF"
          },
          {
            img: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTfejb_WuOSlhXw31HQbQuuKaPNesLz97pyMbMMe1ixHQ&s",
            title: "kahf",
            harga: "Rp 200.000",
            description: "kahf harum alami "
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