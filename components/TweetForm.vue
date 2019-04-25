<template>
<div>
  <v-card-text @click="changeToTextarea">
                <!--여기에는 트위터의 컴포넌트가 들어갈 예정입니다. !-->
      <form id ="tweet_form">
        <v-textarea id="inputEl" label="Outline" placeholder="what's happening?" v-model ="text" single-line outline prepend-icon="account_circle" autofocus v-bind:rows="smile? row1 : row2"></v-textarea>
        <v-btn type="submit" class="submitButton" round color="#f4d041">quack</v-btn>
      </form>
  </v-card-text>
</div>
</template>

<script>
export default {
   components: {
    
  },
  data: () => ({
     text: '',
     row1: 1,
     row2: 10,
     smile: true
  }), 
  methods: {
    changeToTextarea(e){
      console.log(this.smile);
      if(this.smile == true){
        this.smile =false
      }else if(this.smile == false){
        this.smile =true
      }   
    },
    firstTimeClick(e){
      console.log(this.smile);
      this.smile = false
    }
  }
}
</script>