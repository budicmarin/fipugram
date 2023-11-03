<template>
    <div class="row">
      <div class="col-1"></div>
    <div class="col-7">
      <instagram-card v-for="card in cards" :key="card" :info="card"/>
      
    </div>
    <div class="col-3">
     
        </div>
      
    </div>
</template>

<script>
// @ is an alias to /src

import InstagramCard from '@/components/InstagramCard.vue'


let cards=[
  'https://picsum.photos/id/1/400/400',
  'https://picsum.photos/id/2/400/400',
  'https://picsum.photos/id/3/400/400',
];

export default {
  name: 'home',
  data:function(){
    return{
      
      cards: cards,
    };
      
  },
  components: {
    InstagramCard
  }
}
</script>

    InstagramCard