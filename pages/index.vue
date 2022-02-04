<template>
  <div>
    <hero />
    <text-sect>
      <h1>O festiwalu</h1>

      <blockquote>
        Każdy uczeń posiada wiele talentów, ta szkoła potrafi je odkryć i
        rozwinąć
      </blockquote>
      <p>
        - takie hasło przyświecało twórczości pierwszej edycji F.E.T.Y. w roku
        1996, Pani Dorocie Adamusiak. Akcja ta była odpowiedzią na brak
        przedmiotów artystycznych w szkołach średnich. Pierwsze edycje
        skierowane były do uczniów XXVI Liceum Ogólnokształcącego im.
        K.K.Baczyńskiego w Łodzi i obejmowały kategorie: plastyczną,
        fotograficzną i literacką. Kolejne lata to prawdziwy rozkwit,
        popularności i wielkie, wojewódzkie przedsięwzięcie… Nasz Festiwal
        otwiera młodym, zafascynowanym sztuką ludziom drzwi do artystycznego
        środowiska. Stwarza możliwość do skonfrontowania swoich umiejętności z
        rówieśnikami i poddania prac ocenie profesjonalnemu jury. Obecnie
        Festiwal podzielony jest na siedem kategorii: literacką, teatralną,
        muzyczną, plastyczną, fotograficzną, filmową oraz taneczną. Tak szerokie
        podejście do tematu sztuki pozwala na prezentację artystycznego dorobku
        uczniów szkół ponadpodstawowych z województwa łódzkiego w każdej
        dziedzinie. Głównym cele naszego przedsięwzięcia jest propagowanie
        kultury wśród młodzieży, tworzenie szansy na wypowiadanie swoich
        poglądów w niekonwencjonalny sposób.
      </p>
      <p>
        Co roku szczycimy się patronatem między innymi Urzędu Miasta Łodzi oraz
        Prezydenta Miasta Łodzi. Każda edycja ma swoje wiodące hasło, które
        determinuje młodych twórców. Oto kilka przykładów: ,,Dziwny jest ten
        świat”, ,,Po drugiej stronie lustra”, &bdquo;Na jawie&rdquo;, ,,Iluzja”, ,,Z
        przymrużeniem oka…”.
      </p>
      <p>
        Opiekę nad tym projektem sprawują obecnie: Pani Profesor Ilona
        Kolasińska-Wilczek oraz Pani Profesor Beata Sapela.
      </p>
    </text-sect>
    <Footer />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Hero from '~/components/index/hero.vue'
import Footer from '~/components/footer.vue'
import TextSect from '~/components/text-sect.vue'

export default Vue.extend({
  components: { Hero, Footer, TextSect },
  name: 'IndexPage',
})
</script>

<style lang="scss">
* {
  box-sizing: border-box;
}

body {
  width: 100%;
  min-height: 100vh;
}
</style>
