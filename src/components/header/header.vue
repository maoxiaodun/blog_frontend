
<template>
<div id="header">
   <div id="header-left">
       <span id="header-left-user">leon,意难平终将和解</span>   
   </div>
   <div id="header-right">
      <ul id="header-right-ul">
        <li v-for="item in items" :key="item.menuTitle">
         {{ item.menuTitle }}
        </li>
      </ul>
   </div>
</div>
</template>

<script>
  export default {
    name: 'Header',
    data() {
      return {
        items: [
         { menuTitle: '首页' },
         { menuTitle: '碎碎念'},
         { menuTitle: '随笔' }
        ]
      };
    },
  }
</script>

<style scoped>
#header{
    position:fixed;
    margin-top:0;  
    width:100%;
    z-index:9999;
    display: flex;
}
#header-left{
    width: 800px;
    display: flex;
    line-height: 53px;
}
#header-left-user{
   margin-left: 50px;
   font-size: 18px;
   color: #f5f6f7;
   line-height: 53px;
   font-family: "Trebuchet MS", Arial, Helvetica, sans-serif !important;
}

#header-right{
    flex:1;
}
ul{
    list-style-type: none;
}
li{
   display: inline-block;
   margin-left: 20px;
   font-size: 18px;
   color: #f5f6f7;
}
marquee{
    width: 200;
}
</style>