<script>
    export default { 
        // Add Code Here
        // challenge: use array
        data: function(){
        return {
            message: "Choose your favourite fruit:",
            fruit1: "apple",
            fruit2: "orange",
            fruit3: "peach",

            fruits: ["apple","orange","peach"],

        };
        //methods:{
        //    method1{
        //        return "a js function";
        //    }
        //}

    }
    }
</script>

<template>
    <div id="app">
        {{ message }} </br>
        {{ fruit1 }} <input type="radio" name="fruit">
        {{ fruit2 }} <input type="radio" name="fruit">
        {{ fruit3 }} <input type="radio" name="fruit">
        </div>
        <h3> Using Array</h3>
        <span v-for="fruit in fruits">
            {{ fruit }} <input type="radio" name="fruit">
        </span>
    
</template>

<style scoped>
</style>
