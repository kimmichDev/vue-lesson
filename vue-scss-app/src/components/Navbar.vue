<template>
   <div>
      <nav class="navbar navbar-expand-md navbar-dark bg-dark mb-4">
         <div class="container-fluid">
            <a class="navbar-brand" href="#">Top navbar</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
               <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarCollapse">
               <ul class="navbar-nav ms-auto mb-2 mb-md-0">
                  <li class="nav-item">
                     <router-link class="nav-link" aria-current="page" to="/">Home</router-link>
                  </li>
                  <li class="nav-item">
                     <router-link class="nav-link" aria-current="page" to="/about">About</router-link>
                  </li>
                  <li class="nav-item">
                     <router-link class="nav-link" aria-current="page" :to="{name :'Contact'}">Contact</router-link>
                  </li>
               </ul>
            </div>
         </div>
      </nav>
   </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
</style>