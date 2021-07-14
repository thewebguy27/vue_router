<template>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <router-link to="/" class="navbar-brand" href="#">Brand</router-link>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNav">
    <ul class="navbar-nav">
      <li class="nav-item ">
       <router-link :to="{name:'Home'}" active-class="active" class="nav-link">Home</router-link>
      </li>
      <li class="nav-item">
       <router-link :to="{name:'About'}" active-class="active" class="nav-link" >About</router-link>
      </li>
      <li class="nav-item">
       <router-link :to="{name:'Jobs'}" active-class="active" class="nav-link">Jobs</router-link>
      </li>
    </ul>
  </div>
</nav>
</template>
<script>
export default {
    name:'Navbar'
}
</script>