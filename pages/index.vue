
<template>
  <div class="page">
    <section class="section1">
      <div class="container">
       <div class="row">
         <div class="col">
           <img class="logo" src="~/assets/img/logo-open-zaakbrug.svg" alt="Zaakbrug logo"/>
         </div>
         <div class="col">
           <button class="github" id="gh-url" href="#" rel="#">
             <svg class="gh-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32.58 31.77">
               <path d="M16.29,0a16.29,16.29,0,0,0-5.15,31.75c.82.15,1.11-.36,1.11-.79s0-1.41,0-2.77C7.7,29.18,6.74,26,6.74,26a4.36,4.36,0,0,0-1.81-2.39c-1.47-1,.12-1,.12-1a3.43,3.43,0,0,1,2.49,1.68,3.48,3.48,0,0,0,4.74,1.36,3.46,3.46,0,0,1,1-2.18c-3.62-.41-7.42-1.81-7.42-8a6.3,6.3,0,0,1,1.67-4.37,5.94,5.94,0,0,1,.16-4.31s1.37-.44,4.48,1.67a15.41,15.41,0,0,1,8.16,0c3.11-2.11,4.47-1.67,4.47-1.67A5.91,5.91,0,0,1,25,11.07a6.3,6.3,0,0,1,1.67,4.37c0,6.26-3.81,7.63-7.44,8a3.85,3.85,0,0,1,1.11,3c0,2.18,0,3.94,0,4.47s.29.94,1.12.78A16.29,16.29,0,0,0,16.29,0Z"/>
             </svg>
             <span class="span">View on github</span>
           </button>
         </div>
       </div>  
      </div>
    </section>

    <section class="section2">
      <div class="container">
       <div class="row">
         <div class="col">
          <p class="mssg">
            Een vertaler om bestaande applicaties, 
            die het oude zds-standaard praten,
             toch met een zgw-zaaksysteem te laten werken.
            </p>
          <p>
            Powered by the <a class="#" href="#" rel="#">Frank!Framework</a>
          </p>
         </div>
       </div>  
      </div>
    </section>

    <section class="section3">
      <div class="container">
       <div class="row">
         <div class="col">
          <h1 class="nieuws">NIEUWS</h1>
          <p class="nieuws_links">🔗 Borging van Open Zaakbrug</p>
          <p class="nieuws_links">🔗 Súdwest-Fryslân live met OpenZaak en Open Zaakbrug</p>
          <p vclass="nieuws_links"> 🔗 Nieuwsbericht met een hele lange titel zodat hij over 2 regels loopt
             omdat je dan in het design kan zien wat er gebeurt</p>
          <p class="nieuws_links">🔗 Release Open Zaakbrug 2.0</p>
         </div>
       </div>  
      </div>
    </section>
 </div>
</template>

<script>
  import "~/assets/css/style.scss";

export default {
  name: 'IndexPage'
};
</script>
