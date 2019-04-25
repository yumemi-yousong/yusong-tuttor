<template>
    <div class="wrap">
       
            <Home class="tabIcon"/><span class="tabText">HOME</span>

            <Bell class="tabIcon"/><span class="tabText">NOTIFICATIONS</span>

            <Flash class="tabIcon"/><span class="tabText">MOMENTS</span>

            <Message class="tabIcon"/><span class="tabText">MESSAGES</span>

            <div class ="duckIcon"> 
                <Duck class="duck"/>
            </div>
         
    </div>
</template>
<script>
import Duck from '~/assets/icons/duck.svg';
import Bell from '~/assets/icons/bell.svg';
import Flash from '~/assets/icons/flash.svg';
import Home from '~/assets/icons/home.svg';
import Message from '~/assets/icons/message.svg';

export default {
  data() {
    return {
    }
  },
  components: {
    Duck,
    Bell,
    Flash,
    Home,
    Message
  },
  props: {
   
  }
}
</script>

<style>
.wrap{
    display: flex;
    height: 100%;
}
.tabIcon {
   max-width: 100%;
   vertical-align: top;
}
.tabText {
    line-height: 30px;
    vertical-align: bottom;
    margin-right: 1%;
    margin-right: 6px;
}
.duckIcon{
     margin-left: 500px;
}
.duck {
    
}
</style>


