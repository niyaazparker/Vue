<template>
  
    <header>
        <nav class="navbar navbar-expand-md navbar-dark fixed-top bg-dark">
          <div class="container-fluid">
            <a class="navbar-brand" href="#"><img src="..\src\assets\images\payspace-logo-new.webp" width="165"/></a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarCollapse" aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
              <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarCollapse">
              <ul class="navbar-nav me-auto mb-2 mb-md-0">
                <li class="nav-item">
                  <a class="nav-link active" aria-current="page" href="#">SOFTWARE</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link" href="#">COMPARE FEATURES</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">SERVICES</a>
                  </li>
              </ul>
              <form class="d-flex">
                <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
                <button class="btn btn-primary" type="submit">Search</button>
              </form>
            </div>
          </div>
        </nav>
      </header>
    <main>
      <div id="myCarousel" class="carousel slide" data-bs-ride="carousel">
          <div class="carousel-indicators">
            <button type="button" data-bs-target="#myCarousel" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
            <button type="button" data-bs-target="#myCarousel" data-bs-slide-to="1" aria-label="Slide 2"></button>
            <button type="button" data-bs-target="#myCarousel" data-bs-slide-to="2" aria-label="Slide 3"></button>
          </div>
          <div class="carousel-inner">
            <div class="carousel-item active">
              <img src="..\src\assets\images\banner_payroll_small-1.webp"/>      
              <div class="container">
                <div class="carousel-caption text-start">
                  <h1>PAYROLL</h1>
                  <p>Enjoy the best payroll software for small business: easy to manage </p>
                  <p class="mb-5"><a class="btn btn-lg btn-primary" href="#">Speak to a sales consultant</a></p>
                </div>
              </div>
            </div>
            <div class="carousel-item">
            <img src="..\src\assets\images\banner_payroll_small-1.webp"/>        
              <div class="container">
                <div class="carousel-caption text-start">
                  <h1>PAYROLL</h1>
                  <p>Enjoy the best payroll software for small business: easy to manage pay-as-you-go </p>
                  <p class="mb-5"><a class="btn btn-lg btn-primary" href="#">Speak to a sales consultant</a></p>
                </div>
              </div>
            </div>
            <div class="carousel-item">
            <img src="..\src\assets\images\banner_payroll_small-1.webp"/>        
              <div class="container">
                <div class="carousel-caption text-start">
                  <h1>PAYROLL</h1>
                  <p>Enjoy the best payroll software for small business: easy to manage pay-as-you-go true cloud</p>
                  <p class="mb-5"><a class="btn btn-lg btn-primary" href="#">Speak to a sales consultant</a></p>
                </div>
              </div>
            </div>
          </div>
          <button class="carousel-control-prev" type="button" data-bs-target="#myCarousel" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
          </button>
          <button class="carousel-control-next" type="button" data-bs-target="#myCarousel" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
          </button>
        </div>
      
        <div class="container main-content mt-4">

          <div class="row">
              <div class="col-lg-4 col-md-12 col-sm-12 col-12">
                <Counter />
              </div>
          

         
            <div class="col-lg-4 col-md-12 col-sm-12 col-12">
              <LibraryBooks />
            </div>
         

         
            <div class="col-lg-4 col-md-12 col-sm-12 col-12">
              <StringReversal />
            </div>
          </div>

           <hr class="featurette-divider">
           
          <div class="row">
            <div class="col-lg-4">
              <img class="rounded-circle" src="..\src\assets\images\payroll-sb-continious_calcs.webp" width="140" height="140"/>
              <h3 class="mt-3">Easily scale for any size business</h3>
              <p>More and more customers manage their people and their payrolls with this affordable, multi-currency, multi-language, yet easy to use solution. </p>
              <p><a class="btn btn-primary" href="#">View details &raquo;</a></p>
            </div>
            <div class="col-lg-4">
            <img class="rounded-circle" src="..\src\assets\images\payroll-lr-reports.webp" width="140" height="140"/>      
              <h3 class="mt-3">No limits</h3>
              <p>No restrictions on the number of wage types. Unlimited everything! </p>
              <p><a class="btn btn-primary" href="#">View details &raquo;</a></p>
            </div>
            <div class="col-lg-4">
              <img class="rounded-circle" src="..\src\assets\images\payroll-sb-scalability.webp" width="140" height="140"/>      
              <h3 class="mt-3">Continuous calculation</h3>
              <p>No more “last week of the month” rush. You don’t need an official pay run to calculate figures. </p>
              <p><a class="btn btn-primary" href="#">View details &raquo;</a></p>
            </div>
          </div>
      
          <hr class="featurette-divider">
      
          <div class="row featurette align-items-center">
            <div class="col-md-7">
              <h2 class="featurette-heading">Third-party system integration</h2>
              <p class="lead">No more manual integration via Microsoft Excel, text, or delimited files. API web services and webhooks are available to consume to integrate any third-party system. Fully integrated with Xero, Quickbooks accounting, and biometric time and attendance systems. </p>
            </div>
            <div class="col-md-5">
                <img class="rounded-circle" src="..\src\assets\images\Third-Party-Integration-500px.webp" width="100%" height="auto"/>       
            </div>
          </div>
      
          <hr class="featurette-divider">
      
         

          <div class="row featurette align-items-center">
            <div class="col-md-7 order-md-2">
              <h2 class="featurette-heading">No need to define everything from scratch.</h2>
              <p class="lead">All component types (earnings, deductions, fringe benefits, etc.) are linked to tax codes. No need to define how wage types must work and whether they should be taxed or not. This includes pre-defined, automated components for bonus tax spread and automated pay out of bonuses. 
                You can buy PaySpace in the morning and pay your first payslips with our small business payroll software by noon!</p>
            </div>
            <div class="col-md-5 order-md-1">
                <img src="..\src\assets\images\payroll-sb-out-of-the-box.webp" width="100%" height="auto"/>        
            </div>
          </div>
      
          <hr class="featurette-divider">
        </div>

      
    </main>
   
      <footer class="px-3">
        <p class="float-end mb-0"><a class="text-prime" href="#">Back to top</a></p>
        <p class="mb-0">PAYSPACE &copy; 2023   &middot; <a class="text-prime" href="#">Privacy</a> &middot; <a class="text-prime" href="#">Terms</a></p>
      </footer>
 
</template>

<script>
import Counter from './components/Counter.vue';
import StringReversal from './components/Stringreversal.vue';
import LibraryBooks from './components/Books.vue';

export default {
  components: {
    Counter,
    StringReversal,
    LibraryBooks,
  },
};
</script>
