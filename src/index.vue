/**  
  content: 主入口
  author:leon
  create: 2021/03/10
 */

<template>
    <div id="container">
     <v-header></v-header>
     <v-banner></v-banner>
    </div>
</template>

<script>
import Header from '@/components/header/Header';
import Banner from '@/components/banner/Banner'
export default {
    name: 'index',
    components:{
        'v-header':Header,
        'v-banner':Banner,
    }
}
</script>

<style scoped>

</style>