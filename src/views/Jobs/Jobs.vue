<template>
    <h1 class=" text-center">Jobs</h1>
    <div class=" container">
        <div class=" row">
            <div class=" col-12 col-md-10 col-lg-8 offset-lg-2 ">
                <ul class=" list-group text-center font-weight-bold" v-for="job in jobs" :key="job.id">
                    <li class="list-group-item list-group-item-primary">
                        <router-link :to="{name:'JobDetails',params:{id:job.id}}">
                              {{job.title}}
                        </router-link>
                    </li>
                    </ul>
            </div>
        </div>
        
    </div>
</template>
<script>
export default {
    data(){
        return{
            jobs:
            [{id:1,title:'Job 1',details:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis commodi similique cum culpa quas officia asperiores obcaecati quo odio. Ea!'},
            {id:2,title:'Job 2 ',details:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis commodi similique cum culpa quas officia asperiores obcaecati quo odio. Ea!'}]
        }
    }
}
</script>