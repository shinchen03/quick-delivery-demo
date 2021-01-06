<template>
 <el-container>
   <head>
   <link
      rel="stylesheet"
      href="https://use.fontawesome.com/releases/v5.7.1/css/all.css"
      integrity="sha384-fnmOCqbTlWIlj8LyTjo7mOUStjsKC4pOpQbqyi7RrhN7udi9RwhKkMHpvLbHG9Sr"
      crossorigin="anonymous"
    />
   </head>
   <el-header>
    <TopBar/>
   </el-header>
   <el-main style="margin-top:50px"><Login/></el-main>
  </el-container>
</template>

<script>
import Login from './components/HelloWorld.vue'
import TopBar from './components/TopBar.vue'
import Vue from 'vue'
import { Button, Select } from 'element-ui'
import lang from 'element-ui/lib/locale/lang/en'
import locale from 'element-ui/lib/locale'
import Element from 'element-ui'
import './element-variables.scss'


locale.use(lang)
Vue.component(Button.name, Button)
Vue.component(Select.name, Select)
Vue.use(Element)

export default {
  name: 'app',
  components: {
    Login,
    TopBar
  }
}
</script>

