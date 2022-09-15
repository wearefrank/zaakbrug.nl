
<template>
  <div>
    <OzbBackground />
    <header class="container">
      <div class="row flex-nowrap">
        <div class="col-4 d-inline-flex align-items-center">
          <img class="logo" src="~/assets/img/logo-open-zaakbrug.svg" alt="Zaakbrug logo" />
        </div>
        <div class="col-8 d-inline-flex justify-content-end align-items-start">
          <a href="#" class="gh-btn">
            <svg class="gh-btn__icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32.58 31.77">
              <path
                d="M16.29,0a16.29,16.29,0,0,0-5.15,31.75c.82.15,1.11-.36,1.11-.79s0-1.41,0-2.77C7.7,29.18,6.74,26,6.74,26a4.36,4.36,0,0,0-1.81-2.39c-1.47-1,.12-1,.12-1a3.43,3.43,0,0,1,2.49,1.68,3.48,3.48,0,0,0,4.74,1.36,3.46,3.46,0,0,1,1-2.18c-3.62-.41-7.42-1.81-7.42-8a6.3,6.3,0,0,1,1.67-4.37,5.94,5.94,0,0,1,.16-4.31s1.37-.44,4.48,1.67a15.41,15.41,0,0,1,8.16,0c3.11-2.11,4.47-1.67,4.47-1.67A5.91,5.91,0,0,1,25,11.07a6.3,6.3,0,0,1,1.67,4.37c0,6.26-3.81,7.63-7.44,8a3.85,3.85,0,0,1,1.11,3c0,2.18,0,3.94,0,4.47s.29.94,1.12.78A16.29,16.29,0,0,0,16.29,0Z" />
            </svg>
            <span class="gh-btn__text">View on GitHub</span>
          </a>
        </div>
      </div>
    </header>

    <section class="hero">
      <div class="container">
        <div class="row mt-5 mb-5">
          <div class="col-12 col-md-8 col-lg-6 col-xl-5">
            <p>
              Een vertaler om bestaande applicaties,
              die het oude zds-standaard praten,
              toch met een zgw-zaaksysteem te laten werken.
            </p>
            <p>
              Powered by the <a href="https://frankframework.org/">Frank!Framework</a>
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="news">
      <div class="container pb-5">
        <h2>Nieuws</h2>
        <div class="row">
          <div class="col">
            <ul class="news__links">
              <li>
                <a
                  href="https://commonground.nl/blog/view/6a946c44-851a-4a2b-bfaf-8368d886aff7/sudwest-fryslan-live-met-openzaak-en-open-zaakbrug">🔗
                  Súdwest-Fryslân live met OpenZaak en Open Zaakbrug</a>
              </li>
              <li>
                <a href="https://blog.wearefrank.nl/borging-openzaakbrug-integratie-vng">🔗 Borging van Open
                  Zaakbrug</a>
              </li>
              <li>
                <a href="#">🔗 Nieuwsbericht met een hele lange titel zodat hij over 2 regels loopt omdat je dan in het
                  design kan zien wat er gebeurt</a>
              </li>
              <li>
                <a href="#">🔗 Release Open Zaakbrug 2.0</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <section class="description container pb-5">
      <h2>Wat doet de Open Zaakbrug?</h2>
      <p>
        De nieuwe standaard voor het zaakgewijs werken is de <a href="https://vng.nl/projecten/zaakgericht-werken-api">zgw standaard</a>, dit is de opvolger van de Zaak- en
        Documentservices (ZDS) standaard. Om de overstap te maken naar deze nieuwe standaard vinden wij het belangrijk
        om niet meer te investeren in de oude-zds-koppelingen, maar zo snel mogelijk de nieuwe zgw-standaard te
        gebruiken. Om deze reden heeft het team Open Zaakbrug een oplossing om de bestaande applicaties, die de oude
        zds-standaard praten, toch met een zgw-zaaksysteem te laten praten.

        Hiermee kunnen gemeentes de bestaande zaaksgewijswerken applicaties blijven gebruiken en toch overstappen op
        bijvoorbeeld <a href="https://openzaak.org">openzaak</a>. Dit zodat alles blijft draaien en ondertussen de overstap kan worden gemaakt naar de
        nieuwe commonground wereld.

        Door te beginnen met een zgw-zaaksysteem kunnen alle nieuwe domein-specifieke-applicaties via deze nieuwe
        standaard aansluiten en krijgen de leveranciers van de bestaande applicaties de tijd om de ZGW koppeling in te
        bouwen.
      </p>
    </section>

    <section class="presentations">
      <div class="container pb-5">
        <h2>Presentaties</h2>
        <div class="row">
          <div class="col">
            <ul class="news__links">
              <li>
                <a
                  href="https://commonground.nl/blog/view/6a946c44-851a-4a2b-bfaf-8368d886aff7/sudwest-fryslan-live-met-openzaak-en-open-zaakbrug">🔗
                  Súdwest-Fryslân live met OpenZaak en Open Zaakbrug</a>
              </li>
              <li>
                <a href="https://blog.wearefrank.nl/borging-openzaakbrug-integratie-vng">🔗 Borging van Open
                  Zaakbrug</a>
              </li>
              <li>
                <a href="#">🔗 Nieuwsbericht met een hele lange titel zodat hij over 2 regels loopt omdat je dan in het
                  design kan zien wat er gebeurt</a>
              </li>
              <li>
                <a href="#">🔗 Release Open Zaakbrug 2.0</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </section>
   </div>
</template>

<script>
import "~/assets/css/style.scss";
import OzbBackground from "../components/ozb-background.vue";

export default {
  name: "IndexPage",
  components: { OzbBackground }
};
</script>
