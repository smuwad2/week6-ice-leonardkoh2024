<script>
    export default { 
        data() {
            return {
                // Add code here
                id: "demo1",
                isActive: true,
                btnClass: 'btn btn-primary',
                btnClass2: 'btn btn-danger',
            }
        },
        methods: { 
   			// Add code here
            changeColor(){
                this.isActive = !this.isActive;
            }
		}
    }
</script>

<template>
    
    <!-- Modify code here -->
    <div class="container">
        <div v-bind:id="id" class="m-2" :class="{'blueBox': isActive, 'redBox': !isActive}">
            div ID : {{id}} 
        </div>
        
        <button type="button" :class="[isActive ? btnClass : btnClass2]" @click="changeColor()">Change Color</button>
    </div>

</template>

<style scoped>
    .redBox {
        background-color: red;
    }
    .blueBox {
        background-color: blue;
    }
    #demo1 {
        color: white;
    }
</style>
