<template>
    <div class="container">
        <form>
            <label for="input">Please Enter YOur Writin :</label>
            <input type="text" id="input" placeholder="WriteText" v-model.trim="inputer">
            <button class="btn" @click.prevent="additem">Add Item</button>
        </form>
       <div class="item-container">
        <h1
           class="itemm" 
           v-for="item, index in array" 
           :key="item.text" 
           :class="{'list': item.ishow}"
           @click="item.ishow = !item.ishow" >{{ item.text }} 
           <button class="btn-delet" @click="deletItem(index)">X</button>
        </h1>
       
       </div>




    </div>
</template>

<script>

export default{
    
    name:'Counter',
    data() {
        return {
            inputer:'',
            array:[
                {text:'Sattar', ishow: false}
            ],
            
        }
    },
    methods:{
        additem(){
            
           if(this.inputer){
            this.array.push({text:this.inputer, ishow: false})
            this.inputer = ''
           }
        },
        deletItem(index){
     
               this.array.splice(index, 1)
        

        }
        
       
    }
  
  
  
   
}
</script>
<style scoped>
.container{
    width: 100%;
    height: 100vh;
}
form{
    width: 70%;
    margin: auto;
    box-shadow: 0 0 4px black;
    border-radius: 10px;
    padding: .8rem;

}
label{
    font-size: 1.1rem;
    font-family: sans-serif;
    margin: 0 .9rem;
}
input{
    width: 60%;
    padding: .4rem;
    border-radius: 10px;
    box-shadow: 0 0 2px black;
}
input:focus{
    outline: none;
}
.btn{
    border-radius: 8px;
    box-shadow: 0 0 3px black;
    font-size: 1.1rem;
    margin: .9rem auto 0 auto;  
    background-color: #fff;
    padding: .2rem .7rem;
    display: block;
    transition: all .9s;
}
.btn:active{
    transform: scale(.8);
}
.itemm{
    width: 90%;
    padding: 10px;
    box-shadow: 0 0 2px black;
    margin: .6rem;
    display: flex;
    justify-content: space-between;
    border-radius: 4px;
}
.btn-delet{
    background-color: #fff;
    font-size: 1.2rem;
    padding: .3rem;
    border-radius: 50%;
    box-shadow: 0 0 3px black;
    width: 30px;
    height: 30px;
    display: flex;
    justify-content: center;
    align-items: center;
    transition: all .9s;
}
.btn-delet:active{
    transform: scale(.7);
    background-color: red;
    color: white;
}
.list{
    background-color: red;
    text-decoration: line-through 1px white;
    
}
</style>

