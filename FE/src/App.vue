<template>
  <div class="layout" id="app">
    <Header>
      <RealHeader></RealHeader>
    </Header>
    <Content>
      <RealContent></RealContent>
    </Content>
  </div>
</template>

<script>
  import { Header,Content,Footer } from 'iview'
  import RealHeader from '@/components/RealHeader'
  import RealContent from '@/components/RealContent'
export default {
  name: 'App',
  data(){
    return {
      courseCom:''
    }
  },
  components:{
    Header,
    Content,
    Footer,
    RealHeader,
    RealContent
  },
  methods:{
    getCourse(course){
      this.courseCom = course;
    }
  }
}
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    /*margin-top: 60px;*/
  }
  .footer{
    width:100%;
    position: absolute;
    bottom:0;
  }
</style>
