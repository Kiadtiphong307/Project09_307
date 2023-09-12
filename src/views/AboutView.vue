<script setup>
  import {ref} from 'vue'
import shop_value from '../components/shop_value.vue';

const list_shop = ref([
{name: 'สุนทรารมณ์',  price:500, img:"https://scontent.fbkk13-2.fna.fbcdn.net/v/t39.30808-6/327442369_874305543617514_7552528986654738604_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=a2f6c7&_nc_eui2=AeFNdHIyDFw8l9dSHVOxGbtd2Q6BSD08VdDZDoFIPTxV0Jyx8MQf2dauMZCHSslW0V1nOlqKwTeXRF6hl0wVPuBq&_nc_ohc=QGIXLCcANAEAX8oL9of&_nc_ht=scontent.fbkk13-2.fna&oh=00_AfDGtzcszEljTAHl8QKGUijSrx-jt8GwLZ5OZs6OTu4VSQ&oe=64FD9D20", quantity: 0 }, 

{name:'Overnight',  price:750, img:"https://scontent.fbkk13-2.fna.fbcdn.net/v/t39.30808-6/314943429_107842845474701_641691726405226769_n.jpg?stp=cp6_dst-jpg&_nc_cat=107&ccb=1-7&_nc_sid=a2f6c7&_nc_eui2=AeFloVqAmAQK63gBmvRlILSFEYxzLzXtdwsRjHMvNe13C67jqz5C4ozZtnfeVB-bdVvF2m0RlI6vAA4gmgVza1hd&_nc_ohc=JsU_-083hU4AX9u2vHL&_nc_ht=scontent.fbkk13-2.fna&oh=00_AfDn433NRDpL4MAAkFVmrpWijqDVhNrFYXkfdIiOmAr2pw&oe=64FDD6B1", quantity: 0 },

{name:'Tamma',      price:1500, img:"https://scontent.fbkk13-2.fna.fbcdn.net/v/t39.30808-6/361305041_779199773993037_7111305937619716444_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=a2f6c7&_nc_eui2=AeGZ36SZ7tHE4Sn56ahHG-4VKhovrXyAa8YqGi-tfIBrxqe1tPcilruoK6M8iPurXs2EtvRAUFDpW4HyLULu-tZG&_nc_ohc=NUl9gU8b32gAX_PJpz-&_nc_ht=scontent.fbkk13-2.fna&oh=00_AfA2l1ggQGMrfsjdgRgq6o2Vr20QfaEeiIvMAwIHJ_KcXQ&oe=64FF0047", quantity: 0 },

{name:'ไปยาล',     price:1599, img:"https://scontent.fbkk13-2.fna.fbcdn.net/v/t39.30808-1/326435697_501993212005268_2267045348590722770_n.jpg?stp=dst-jpg_p320x320&_nc_cat=103&ccb=1-7&_nc_sid=754033&_nc_eui2=AeGmFPzsMIq3BFoj1PViby3YxTbvRg4F5HPFNu9GDgXkc_ntcZ1iiswsTq9-jcH-pP3KvXD7sj7D6hgpksqlR7X8&_nc_ohc=w70TqL0LBHMAX9eRmtz&_nc_ht=scontent.fbkk13-2.fna&oh=00_AfDtcL42wBIGzSJBRdL2HOvzWz8Iouxb-CLNFaSsdyGKeQ&oe=64FDEFC9", quantity: 0 },

{name:'Too nice',    price:1699, img:"https://scontent.fbkk13-2.fna.fbcdn.net/v/t39.30808-6/292496235_1007767096737663_225747972753273688_n.png?_nc_cat=110&ccb=1-7&_nc_sid=a2f6c7&_nc_eui2=AeElcXBRemzlCc00lIr4Gg4HzTWRn5lngH3NNZGfmWeAfdM0r7nLsyIZaexMz8_UB8jL6tg2M4vxxRmT3iKLZbmm&_nc_ohc=R0AqwtXy2XQAX-6usnI&_nc_ht=scontent.fbkk13-2.fna&oh=00_AfCKCH-GD6spsF2crGqpoQLClRFzW_2zxeLiQdyhl16SXQ&oe=64FDB576", quantity: 0 },


{name:'ท่าช้าง',  price:1890,  img:"https://scontent.fbkk13-2.fna.fbcdn.net/v/t39.30808-6/350942472_940270750565444_6986476706008406745_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=a2f6c7&_nc_eui2=AeGOw7uk2VFH7K0Y1VV60YyZJnOKgtUtkswmc4qC1S2SzHt3w5MKrvNCf6Jeuix0rENdMiRxxWccKJITy2tbgpFm&_nc_ohc=EBl4NSGR99UAX9T9gPf&_nc_ht=scontent.fbkk13-2.fna&oh=00_AfCxWFHC52mx2q6QlRYlCfWtamuHpgvz2Rl7wsWrb3JeQw&oe=64FE7920", quantity: 0 },


{name:'Beer lab',      price:675, img:"https://scontent.fbkk13-2.fna.fbcdn.net/v/t39.30808-6/326776461_983306725977390_1286925122631726978_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=a2f6c7&_nc_eui2=AeF1Ywb4j0jzAKiBj2OSSgPDDbJxNGoeGtoNsnE0ah4a2rGXYUI_AKkz9jMg_OiM6XP4-mQuh4pgkXOJfXGs7H2T&_nc_ohc=C2NpKwZz5ZcAX-iRwGx&_nc_ht=scontent.fbkk13-2.fna&oh=00_AfCGwZMuYRbBc1i9Ivz1WNNLf6IBiCJgzMhZd5ZieomqYQ&oe=64FE3E79", quantity: 0 },


{name:'Warm up',     price:1250, img:"https://scontent.fbkk13-2.fna.fbcdn.net/v/t39.30808-6/326148970_1521569305000988_2338094468162899732_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=a2f6c7&_nc_aid=0&_nc_eui2=AeHdrRzQLjAXk3z9zYSatohZJSB-z1el8TIlIH7PV6XxMsYI3VPYXaWft8sKQRkEMdnn378aOgRBez-gwkIXATgA&_nc_ohc=-nloMFue0PQAX-oPt_-&_nc_ht=scontent.fbkk13-2.fna&oh=00_AfBXrWHaV-03hPUW252v3dkcfrL-3dEN5uWBqRGG3hOVzw&oe=64FF1E18", quantity: 0 },
])
</script>







<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
<div v-for=" (shop,index) in list_shop" :key="index" >
  <shop_value
    :name = "shop.name"
    :price = "shop.price"
    :image = "shop.img"
  ></shop_value>
  </div>


  
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}

</style>
