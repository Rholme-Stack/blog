<template>
    
    <NavBar/>
    

    <div class="d-flex">
        <div class="col-4">
            <EntryList/>

        </div>
        <div class="col-8" >
            <router-view />
        </div>

    </div>
    
    
</template>

<script lang="ts">
import { defineAsyncComponent } from "vue";





export default{
    components: {
        NavBar: defineAsyncComponent(()=> import('../components/NavBar.vue')),
        EntryList: defineAsyncComponent(()=> import('../components/EntryList.vue')),
        
    }
}

</script>