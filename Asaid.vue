<template>
    <div class="my-8  flex flex-col items-center justify-center text-center font-[Dana]">

        <div>
            <h1 class="text-2xl"><span class="text-rose-600">اینجا برترین ها </span>حضور دارند برای شما</h1>
            <br>
            <p>شایان مصلح، شماره پیراهنش در پرسپولیس را برای گرامی‌داشت قربانیان زمین‌لرزه رودبار و منجیل، ۶۹ انتخاب کرده بود؟</p>
        </div>
        
        <div class="grid md:grid-cols-4 gap-1 mr-8 md:mx-10 my-10" data-aos="flip-up" data-duration="500">

            <div data-aos="flip-left" data-duration="600" class="w-[80%] flex flex-col py-10 justify-center items-center gap-6 border border-t-8 rounded-lg border-rose-500 my-6 p-3 hover:text-black hover:bg-rose-500 transition-all duration-200">
                <h2 class="text-2xl">{{ startup }} </h2>
                <p><span class="text-2xl mx-2">15000</span>تومان</p>
                <p class="text-2xl border-b-2 border-rose-600">ماهانه</p>
                <h2 class="text-2xl text-rose-600">متخصصین</h2>
                <p>توسط شارل-آنتوان کامبون برای پردهٔ ۳ از صحنهٔ سوم اُپِرای رابرت بروس (en) اثر مشترک جواکینو روسینی و لویی نیدرمایر.</p>
                <button class="btn-1">خرید سرویس</button>
            </div>

            <div data-aos="flip-up" data-duration="600" class="w-[80%] my-6 flex flex-col py-10 justify-center items-center gap-6 border rounded-lg border-t-8 border-rose-500 p-3 hover:text-black hover:bg-rose-500 transition-all duration-200">
                <h2 class="text-2xl">{{ ai }} </h2>
                <p><span class="text-2xl mx-2">10000</span>تومان</p>
                <p class="text-2xl border-b-2 border-rose-600">هفتگی</p>
                <h2 class="text-2xl text-rose-600">پزشک ها</h2>
                <p>توسط شارل-آنتوان کامبون برای پردهٔ ۳ از صحنهٔ سوم اُپِرای رابرت بروس (en) اثر مشترک جواکینو روسینی و لویی نیدرمایر.</p>
                <button class="btn-1">خرید سرویس</button>
            </div>

            <div data-aos="flip-down" data-duration="600" class="w-[80%] my-6 flex flex-col py-10 justify-center items-center gap-6 border rounded-lg border-t-8 border-rose-500 p-3 hover:text-black hover:bg-rose-500 transition-all duration-200">
                <h2 class="text-2xl">{{ engineer }} </h2>
                <p><span class="text-2xl mx-2">25000</span>تومان</p>
                <p class="text-2xl border-b-2 border-rose-600">روزانه</p>
                <h2 class="text-2xl text-rose-600">تاجران</h2>
                <p>توسط شارل-آنتوان کامبون برای پردهٔ ۳ از صحنهٔ سوم اُپِرای رابرت بروس (en) اثر مشترک جواکینو روسینی و لویی نیدرمایر.</p>
                <button class="btn-1">خرید سرویس</button>
            </div>

            <div data-aos="flip-right" data-duration="600" class="w-[80%] my-6 flex flex-col py-10 justify-center items-center gap-6 border rounded-lg border-t-8 border-rose-500 p-3 hover:text-black hover:bg-rose-500 transition-all duration-200">
                <h2 class="text-2xl">{{ bussines }} </h2>
                <p><span class="text-2xl mx-2">19000</span>تومان</p>
                <p class="text-2xl border-b-2 border-rose-600">ماهانه</p>
                <h2 class="text-2xl text-rose-600">وزیران</h2>
                <p>توسط شارل-آنتوان کامبون برای پردهٔ ۳ از صحنهٔ سوم اُپِرای رابرت بروس (en) اثر مشترک جواکینو روسینی و لویی نیدرمایر.</p>
                <button class="btn-1">خرید سرویس</button>
            </div>
            

        </div>

    </div>
</template>

<script>
export default {
    name:'Asaid',
    data() {
        return {
            startup:'استارت اپ',
            bussines:'بیزنس',
            engineer:'مهندسین',
            ai:'هوش مصنوعی'
            
        }
    },
}
</script>