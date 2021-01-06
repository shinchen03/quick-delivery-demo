<template>
 <el-container>
   <el-header>
    <TopBar/>
   </el-header>
   <el-main><HelloWorld msg="Welcome to Your Vue.js App"/></el-main>
  </el-container>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
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
    HelloWorld,
    TopBar
  }
}
</script>

