<template>
    <h1 class=" text-center mt-2">
        Job Details Page
    </h1>
    <p>The Job id is {{id}}</p>
</template>
<script>
export default {
    props:['id']    
    // data(){
    //     return{
    //         id:this.$route.params.id
    //     }
    // }
}
</script>