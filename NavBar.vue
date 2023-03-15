<template>
    <div class="parent-navbar" >

        <div class="left-navbar" >
            <div>
                <button class="btn-1">{{ firstbtn }} </button>
                <button class="btn-2">{{ loginbtn }} </button>
            </div>

           <ul class="ul-list">
                  <li class="active-item"><a href="#">{{ loginpage }}</a></li>
                  <li class="item-list relative" :class="{'active-item' : isshow}"><a href="#" @click="isshow = !isshow">{{kala }}<i class="fas fa-chevron-down mx-2"></i></a>

                  <ul class="dropdown" v-show="isshow">
                    <li class="pt-5"><a href="#">{{ farhangi }}</a></li>
                    <li class="pt-5"><a href="#">{{  amozeshi }}</a></li>
                    <li class="pt-5"><a href="#">{{ tafrihi }}</a></li>
                  </ul>

                  </li>
                  <li class="item-list"><a href="#">{{ aboutwe }}</a> </li>
                  <li class="item-list relative" :class="{'active-item' : ishide}"  @click="ishide = !ishide"><a href="#">{{ callwe }}<i class="fas fa-chevron-down mx-2"></i></a>
                  
                    <ul class="dropdown-2" v-show="ishide">
                    <li class="pt-5"><a href="#"> ایجاد </a></li>
                    <li class="pt-5"><a href="#"> پرداخت </a></li>
                    <li class="pt-5"><a href="#"> فروش </a></li>
                  </ul>

                   </li>
           </ul>
        </div>

        <div class="md:hidden" @click="ismobil=!ismobil">
            <div class="bar-menu">
                <i class="fas fa-bars text-xl"></i>
            </div>     
        </div>


        <div class="mobil-list" v-show="ismobil">

                <ul class="list">
                  <li><a href="#">{{ loginpage }}</a></li>
                  <li :class="{'active-item' : isshow}"><a href="#" @click="isshow = !isshow">{{kala }}<i class="fas fa-chevron-down mx-2"></i></a>

                  <ul v-show="isshow">
                    <li class="pt-5"><a href="#">{{ farhangi }}</a></li>
                    <li class="pt-5"><a href="#">{{  amozeshi }}</a></li>
                    <li class="pt-5"><a href="#">{{ tafrihi }}</a></li>
                  </ul>

                  </li>
                  <li><a href="#">{{ aboutwe }}</a> </li>
                  <li :class="{'active-item' : ishide}"  @click="ishide = !ishide"><a href="#">{{ callwe }}<i class="fas fa-chevron-down mx-2"></i></a>
                  
                    <ul v-show="ishide">
                    <li class="pt-5"><a href="#"> ایجاد </a></li>
                    <li class="pt-5"><a href="#"> پرداخت </a></li>
                    <li class="pt-5"><a href="#"> فروش </a></li>
                  </ul>

                   </li>
                </ul>

                <div class="btns">
                  <button class="btn-1">{{ firstbtn }} </button>
                  <button class="btn-2">{{ loginbtn }} </button>
                </div>


        </div>        


        <div class="right-navbar" data-aos="flip-right" data-duration="400">
            <span class="icon" @click="toggleTheme" v-show="this.show == 'dark'"><i class="fa-solid fa-moon"></i></span>
            <span class="icon" @click="lightHandel"  v-show="this.show == 'light'"><i class="fa-solid fa-sun"></i></span>
            <h1>WebProg.io</h1>
        </div>

    </div>
    
</template>

<script>
import { init } from 'events';

   

export default{

   
    name:'NavBar',
    data(){
        return{
            firstbtn:'عضویت',
            loginbtn:'ورود',
            loginpage:'صفحه اصلی',
            kala:'محصولات',
            aboutwe:'درباره ما',
            callwe:'تماس با ما',
            farhangi:'محصولات فرهنگی',
            amozeshi:'محصولات اموزشی',
            tafrihi:'محصولا تفریحی',
            isshow:false,
            ishide:false,
            ismobil:false,
            isDarkMode:false,
            show:'dark',
          
        }
        
        
    },
    methods:{
      toggleTheme(){
        const html = document.querySelector('html');
        if(!this.isDarkMode){
          html.classList.add('dark');
          this.isDarkMode=true;
          this.show = 'light';
        }
        
      },
      // init(){
      //   if(localStorage.theme === 'dark'){
      //     this.isDarkMode = true
      //   }
      // },
      lightHandel(){
        const html = document.querySelector('html');
        
        html.classList.remove('dark');
        this.isDarkMode=false;
        if(this.show == 'light'){
          this.show = 'dark'}
        
      },
      
      

    }
    
   
}

</script>