<script>
import TheHeader from "../components/TheHeader.vue";
import TheFooter from "../components/TheFooter.vue";

export default {

  components: {
    TheHeader,
    TheFooter
  },

  methods: {
    redirectToCocktails() {
      this.$router.push({ name: 'cocktails' })
    }
  }

}
</script>

<template>
  <TheHeader></TheHeader>
  <main>
    <div>
      <div class="bg-container-fluid">
        <div class="row ">
          <div class="col-12 col-md-6"></div>
          <div class="col-12 col-md-6 mt-5 pt-5">
            <div class="text-container p-4 text-white text-center pt-5">
              <h1 class="mt-5">Boolean Cocktail Bar</h1>
              <br>
              <p class="custom-font text-center mt-2 ">Benvenuti a boolean, il cocktail bar che unisce
                <br>l'arte dei cocktail alla logica booleana.<br>
                Scoprite nuovi sapori e contattateci per informazioni.
              </p>
              <div>
                <button class="btn m-3 button-color" @click="redirectToCocktails">I NOSTRI COCKTAIL</button>

              </div>
              <div class="col-6 col-md-6 d-flex mt-5 pt-5">


              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>
  <TheFooter></TheFooter>
</template>

<style>
main {
  background-image: url(../assets/img/home-page-cocktailbar.jpg);
  background-size: cover;
  background-position-x: left bottom;
  background-position-y: bottom;
  background-repeat: no-repeat;
  height: 80vh;
}

.button-color {
  background-color: #A3A656;
}
.custom-font{
  font-size: 1.5rem;
}
</style>