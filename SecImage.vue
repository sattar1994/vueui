<template>
    <div class="my-8 font-[Dana] text-center text-2xl">
        <div>
            <h1>اینجا شما میتوانید مشاهده کنید <span class="text-rose-600">برترین ها رو</span></h1>
            <p class="text-[1.1rem] my-2">با رشد روزافزون این دانشنامه گردانندگان آن در بنیاد ویکی‌مدیا چندین پروژهٔ مشابه دیگر همچون و ویکی‌داده و ویکی‌گونه را پدیدآوردند.</p>
        </div>

        <div class="text-[1rem] flex justify-center gap-3">
            <button class="btn-1 my-5" :class="{'back' : istabiat}" @click="tHandel">{{ tabiat }}</button>
            <button class="btn-1 my-5" :class="{'back' : istekno}" @click="teknoHandel">{{ tekno }}</button>
            <button class="btn-1 my-5" :class="{'back' : istravel}" @click="traHandel">{{ travel }}</button>
            <button class="btn-1 my-5" :class="{'back' : isall}" @click="allHandel">{{ all }}</button>
        </div>


        <div data-aos="flip-left" data-duration="500" class="md:flex md:justify-between my-5 p-3 transition-all duration-200" v-show="ispart === 'tabiatt'">
            <img data-aos="flip-left" data-duration="600" src="../image/tabiat1.jpg" class="md:w-[30%] my-2 rounded-lg">
            <img data-aos="flip-up" data-duration="600" src="../image/tabiat2.jpg" class="md:w-[30%] my-2 rounded-lg">
            <img data-aos="flip-down" data-duration="600" src="../image/tabiat3.jpg" class="md:w-[30%] my-2 rounded-lg">
        </div>

        <div data-aos="flip-up" data-duration="500" class="md:flex md:justify-between my-5 p-3 transition-all duration-200" v-show="ispart === 'teknoo'">
            <img src="../image/tekno1.jpg" class="md:w-[30%] my-2 rounded-lg">
            <img src="../image/tekno2.jpg" class="md:w-[30%] my-2 rounded-lg">
            <img src="../image/tekno3.jpg" class="md:w-[30%] my-2 rounded-lg">
        </div>

        <div data-aos="fade-up" data-duration="500" class="md:flex md:justify-between my-5 p-3 transition-all duration-200" v-show="ispart === 'travell'">
            <img src="../image/travel.jpg" class="md:w-[30%] my-2 rounded-lg">
            <img src="../image/travel (2).jpg" class="md:w-[30%] my-2 rounded-lg">
            <img src="../image/travel3.jpg" class="md:w-[30%] my-2 rounded-lg">
        </div>

        <div data-aos="flip-down" data-duration="500" class="md:flex md:justify-between my-5 p-3 flex-wrap transition-all duration-200" v-show="ispart === 'alll'">

            <img src="../image/tabiat1.jpg" class="md:w-[30%] my-2 rounded-lg">
            <img src="../image/tabiat2.jpg" class="md:w-[30%] my-2 rounded-lg">
            <img src="../image/tabiat3.jpg" class="md:w-[30%] my-2 rounded-lg">

            <img src="../image/tekno1.jpg" class="md:w-[30%] my-2 rounded-lg">
            <img src="../image/tekno2.jpg" class="md:w-[30%] my-2 rounded-lg">
            <img src="../image/tekno3.jpg" class="md:w-[30%] my-2 rounded-lg">

            <img src="../image/travel.jpg" class="md:w-[30%] my-2 rounded-lg">
            <img src="../image/travel (2).jpg" class="md:w-[30%] my-2 rounded-lg">
            <img src="../image/travel3.jpg" class="md:w-[30%] my-2 rounded-lg">

        </div>

        

        
    </div>
</template>

<script>
export default {
    name:'SecImage',
    data() {
        return {
            tabiat:'طبیعت',
            tekno:'تکنولوزی',
            travel:'مسافرت',
            all:'همه',
            ispart:'tabiatt',
            istabiat:true,
            istekno:false,
            istravel:false,
            isall:false,
           
            
            
        }
    },
    methods:{
        tHandel(){
            this.ispart = 'tabiatt'
            this.istabiat=!this.istabiat
            this.istekno=false
            this.istravel=false
            this.isall=false
        },
        teknoHandel(){
            this.ispart='teknoo'
            this.istekno=!this.istekno
            this.istravel=false
            this.isall=false
            this.istabiat=false

        },
        traHandel(){
            this.ispart = 'travell'
            this.istravel=!this.istravel
            this.isall=false
            this.istabiat=false
            this.istekno=false
        },
        allHandel(){
            this.ispart= 'alll'
            this.isall=!this.isall
            this.istabiat=false
            this.istekno=false
            this.istravel=false
        }
       
    }
}
</script>