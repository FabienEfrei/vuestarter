<template>
  <div>  
    <h1>{{ title + i+ times}}</h1>
    <button @click="iAmClicked()">Click if you can!</button>
  </div>
</template>
 
<script>
    export default {
       
        data() {
            return {
                title: 'you are a boss and you have cliked : ',
                i : 0 ,
                times :" times",
            }
        },
        methods: {

        
            iAmClicked() {
                this.i +=1;
                this.title = "you are a boss and you have cliked : ";
                this.times =" times";
            },

           
        }
    };
</script>