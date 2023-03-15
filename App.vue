<template>
  <div id="app" class="overflow-hidden">
    <NavBar />
    <Main data-aos="fade-down" data-aos-duration="400"/>
    <Section data-aos="fade-right" data-aos-duration="500"/>
    <Asaid data-aos="fade-left" data-aos-duration="600"/>
    <SecImage data-aos="fade-up-right" data-aos-duration="700"/>
    <Input data-aos="fade-down-left" data-aos-duration="600"/>
    <Footer data-aos="flip-left" data-aos-duration="500"/>
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue';
import Main from './components/Main.vue';
import Section from './components/Section.vue';
import Asaid from './components/Asaid.vue';
import Footer from './components/Footer.vue';
import SecImage from './components/SecImage.vue';
import Input from './components/Input.vue'

export default {
  
  name: 'App',
  components:{NavBar, Main, Section, Asaid, Footer, SecImage, Input}
 
}
</script>



