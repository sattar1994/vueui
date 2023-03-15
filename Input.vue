<template>
    <div class="my-8 px-2">
        <div style="height: 50px; overflow: hidden;" ><svg viewBox="0 0 500 150" preserveAspectRatio="none" style="height: 100%; width: 100%;"><path d="M16.64,30.11 C71.95,258.06 295.99,-112.97 500.00,49.98 L500.00,150.00 L-3.67,156.42 Z" style="stroke: none; fill: rgb(244 63 94);"></path></svg></div>

         <div class="md:grid md:grid-cols-2 gap-2 font-[Dana] px-6">

            <div class="flex flex-col gap-8 my-4">
                <h1 class="text-2xl border-b-2 border-rose-700 text-center md:w-[40%] py-2">فرم ثبت نام کابران</h1>
                <p class="text-[1.2rem]">اینجا شما میتوانید به راحتی ثبت نام کنید و دسترسی کامل داشته باشید به همه امکانات وب سایت</p>

                <p>
                    ایمیل: <br>
                    <input  class="border-2 border-gray-400 md:w-[50%] rounded-md px-3" placeholder="ایمیل..."/>
                </p>
                <p>
                    متن پیام: <br>
                    <textarea class="border-2 border-gray-400 md:h-32 rounded-md md:w-[50%] px-3" placeholder="متن پیام..."/>
                </p>

             
              <!-- <button class="btn-2">jkjkj</button> -->
            <button class="btn-2 text-center md:w-[15%] rounded-full">ارسال پیام</button>
            </div>

            <div class="flex justify-end">
                <img src="../image/vector.png" class="md:w-[60%] md:h-78 rounded-full " />
            </div>
         </div>

        <div style="height: 50px; overflow: hidden;" ><svg viewBox="0 0 500 150" preserveAspectRatio="none" style="height: 100%; width: 100%;"><path d="M0.00,49.98 C334.36,287.67 271.49,-49.98 528.49,206.75 L500.00,0.00 L0.00,0.00 Z" style="stroke: none; fill: rgb(244 63 94);"></path></svg></div>
        
    </div>
</template>

<script>

export default {
    name:'Input',
    data(){
        return{

        }
    }
}
</script>