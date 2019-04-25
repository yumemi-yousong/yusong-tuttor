<template>
  <v-app>
    <!--header!-->
    <v-toolbar prominent>
        <span>  
          <PageTab></PageTab>
        </span>  
        <v-spacer></v-spacer>  
        <input type="search" placeholder="Search Tuttor" class="search_input"><v-icon>search</v-icon>
      <div class="dropdown">
        <v-btn class="dropbtn" depressed fab><Profilepic></Profilepic></v-btn>
            <div class="dropdown-content">
              <a href="#">Link 1</a>
              <a href="#">Link 2</a>
              <a href="#">Link 3</a>
            </div>
      </div> 
      
        <v-btn round color="#f4d041">Quack</v-btn> 
    </v-toolbar>
    <!--여기 부분이 인덱스로 들어가는 부분!-->
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
  
  </v-app>
</template>

<script>
import Profilepic from '~/components/Profilepic';
import PageTab from '~/components/Header/PageTabs/index';

export default {
  data() {
    return {
      
    }
  },
  components: {
    Profilepic,
    PageTab
  },
  props: {
   
  }
}

</script>
<style lang="stylus">
   .group
    display: flex
    justify-content: space-around

</style>
<style>
  .search_input {
    float: right;
    border-radius: 10px;
    box-sizing: border-box;
    color: #14171a;
    display:block;
    font-size: 12px;
    height: 32px;
    line-height: 16px;
    padding: 8px 0px 8px 0px;
  }
  .dropbtn{
    color: white;
    padding: 16px;
    font-size: 16px;
    border: none;
    cursor: pointer;
  }
  .dropdown-content {
    display: none;
    position: absolute;
    background-color: #f9f9f9;
    min-width: 160px;
    box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
    z-index: inherit;
  }
  .dropdown:hover .dropdown-content{
     display: block;
  }
  .dropdown {
    position: relative;
    display: inline-block;
  }
  .dropdown-content a {
    color: black;
    padding: 12px 16px;
    text-decoration: none;
    display: block;
  }
  .dropdown-content a:hover {background-color: #f1f1f1}
</style>


