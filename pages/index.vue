<template>
  
  <div class="whole_div">
      <div class="card_group">
        <div class="left_list">
          <ProfileCard></ProfileCard>
          <TrendsCard></TrendsCard>
          <SneakCard></SneakCard>
        </div>
        <div class="center_list">
          <v-card class="center_card">
            <TweetForm></TweetForm>
          </v-card>
        </div>
        <div class="right_list"> 
          
        </div>
      </div>
  </div>
  
</template>

<script>
import ProfileCard from '~/components/ProfileCard';
import Profilepic from '~/components/Profilepic';
import TrendsCard from '~/components/TrendsCard';
import SneakCard from '~/components/SneakCard';
import TweetForm from '~/components/TweetForm';

export default {
  components: {
    ProfileCard,
    Profilepic,
    TrendsCard,
    SneakCard,
    TweetForm
  },
  data: () => ({
     msg: 'hello'
  }), 
  methods: {
   
  }
}
</script>
<style>
    .card_group{
      display: flex;
      position: relative;
    }
    .left_list {
      margin: 10px;
      height: 45%;
      width: 15%;
    }
    .center_list { 
      margin: 10px;
      width: 70%;
      height: 70%;
    }
    .center_card {
      margin: 20px;
    }
    .right_card {
      margin: 20px;
    }
    .right_list {
      margin: 10px;
      height: 45%;
      width: 15%;
    }
 
</style>

