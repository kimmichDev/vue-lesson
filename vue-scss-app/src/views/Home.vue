<template>
   <div class="container">
      <div class="row justify-content-center">
         <div class="col-12 col-lg-6">
            <div id="myC" class="carousel slide" data-bs-ride="carousel">
               <div class="carousel-indicators">
                  <button type="button" data-bs-target="#myC" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
                  <button type="button" data-bs-target="#myC" data-bs-slide-to="1" aria-label="Slide 2"></button>
                  <button type="button" data-bs-target="#myC" data-bs-slide-to="2" aria-label="Slide 3"></button>
               </div>
               <div class="carousel-inner">
                  <div class="carousel-item active">
                     <img
                        src="https://images.unsplash.com/photo-1630576904866-d51b579796f8?ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHw1M3x8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60"
                        class="d-block"
                        height="500"
                        alt
                     />
                  </div>
                  <div class="carousel-item">
                     <img
                        src="https://images.unsplash.com/photo-1630576904866-d51b579796f8?ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHw1M3x8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60"
                        class="d-block"
                        height="500"
                        alt
                     />
                  </div>
                  <div class="carousel-item">
                     <img
                        src="https://images.unsplash.com/photo-1630576904866-d51b579796f8?ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHw1M3x8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60"
                        class="d-block"
                        height="500"
                        alt
                     />
                  </div>
               </div>
               <button class="carousel-control-prev" type="button" data-bs-target="#myC" data-bs-slide="prev">
                  <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                  <span class="visually-hidden">Previous</span>
               </button>
               <button class="carousel-control-next" type="button" data-bs-target="#myC" data-bs-slide="next">
                  <span class="carousel-control-next-icon" aria-hidden="true"></span>
                  <span class="visually-hidden">Next</span>
               </button>
            </div>
            <button class="btn btn-primary mt-3 me-2" @click="next()">Next</button>
            <button class="btn btn-primary mt-3" @click="hideC()">Show/Hide</button>
         </div>
      </div>
   </div>
</template>

<script>
export default {
   methods: {
      next() {
         let myCarousel = $("#myC");
         let carousel = new bootstrap.Carousel(myCarousel, {
            interval: 1000,
         });
         carousel.next();
         console.log(myCarousel);
      },
      hideC() {
         $("#myC").toggle("slow");
      },
   },
};
</script>

<style lang="scss">
</style>