<template>
  <div>
    <div class="container-nero">
      <CardDc
      v-for="objDc in arrDc"
      :key=objDc.titolo
      :cartella=" objDc"
      class="card-dc"
      />
    </div>
    <div class="container-blu">
      <div class="ima">
        <img src="./img/buy-comics-digital-comics.png" alt="" />
        DIGITAL COMICS
      </div>
      <div class="ima">
        <img src="./img/buy-comics-merchandise.png" alt="" />
        DC MERCHANDAISE
      </div>
      <div class="ima">
        <img src="./img/buy-comics-shop-locator.png" alt="" />
        SUBSCRIPTION
      </div>
      <div class="ima">
        <img src="./img/buy-comics-subscriptions.png" alt="" />
        COMICH SHOP
      </div>
      <div class="ima">
        <img src="./img/buy-dc-power-visa.svg" alt="" />
        DC POWER VISA
      </div>
    </div>
    <div class="parte-dc">
      <div class="box-list">
        <ul>
          <h4>DC COMCIS</h4>
          <li>lorem</li>
          <li>lorem</li>
          <li>lorem</li>
        </ul>
        <ul>
          <h4>DC</h4>
          <li>lorem</li>
          <li>lorem</li>
          <li>lorem</li>
          <li>lorem</li>
          <li>lorem</li>
        </ul>
        <ul>
          <h4>SITES</h4>
          <li>lorem</li>
          <li>lorem</li>
          <li>lorem</li>
        </ul>
      </div>
      <div><img src="./img/dc-logo-bg.png" alt="" /></div>
    </div>
  </div>
</template>

<script>
import CardDc from "@/components/CardDc.vue"
export default {
  name: "MainPage",
  components: {
    CardDc,
  },
  data(){
    return {
      arrDc: [
      {
    thumb:
    "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
    price: "$19.99",
    series: "Action Comics",
    type: "comic book",
    },
    {
    thumb:
    "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
    price: "$3.99",
    series: "American Vampire 1976",
    type: "comic book",
    },
    {
    thumb:
    "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
    price: "$16.99",
    series: "Aquaman",
    type: "graphic novel",
    },
    {
    thumb:
    "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
    price: "$2.99",
    series: "Batgirl",
    type: "comic book",
    },
    {
    thumb:
    "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    price: "$3.99",
    series: "Batman",
    type: "comic book",
    },
    {
    thumb:
    "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    price: "$2.99",
    series: "Batman Beyond",
    type: "comic book",
    },
    {
    thumb:
    "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
    price: "$3.99",
    series: "Batman/Superman",
    type: "comic book",
    },
    {
    thumb:
    "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
    price: "$4.99",
    series: "Batman/Superman Annual",
    type: "comic book",
    },
    {
    thumb:
    "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
    price: "$5.99",
    series: "Batman: The Joker War Zone",
    type: "comic book",
    },
    {
    thumb:
    "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
    price: "$6.99",
    series: "Batman: Three Jokers",
    type: "comic book",
    },
    {
    thumb:
    "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
    price: "$4.99",
    series: "Batman: White Knight Presents: Harley Quinn",
    type: "comic book",
    },
    {
    thumb:
    "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
    price: "$16.99",
    series: "Catwoman",
    type: "graphic novel",
    },
      ]
    }
  }
};
</script>

<style lang="scss" scoped>
.container-nero {
  background-color: black;
  height: 70vh;
  color: white;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  margin: 0 auto;
  padding: 0 1rem;
  .card-dc {
    flex: 0 0 25%;
  }
}

.container-blu {
  background-color: rgba(2, 130, 249, 255);
  height: 15vh;
  color: white;
  display: flex;
  justify-content: space-around;
  align-items: center;
  .ima {
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 10px;
    gap: 5px;
  }
}
img {
  height: 50px;
}
.parte-dc {
  background-image: url("./img/footer-bg.jpg");
  height: 45vh;
  display: flex;
  color: white;
  justify-content: space-around;
  align-items: center;
  img {
    height: 300px;
  }
  .box-list {
    display: flex;
    gap: 30px;
  }
  ul li {
    list-style-type: none;
    color: gray;
  }
}
</style>
