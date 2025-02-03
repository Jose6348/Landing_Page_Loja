<template>
  <div id="app">
    <Header />
    <main>
      <HeroSection />
      <FeaturesSection />
      <CtaSection />
      <ContactForm />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import HeroSection from './components/HeroSection.vue'
import FeaturesSection from './components/FeaturesSection.vue'
import CtaSection from './components/CtaSection.vue'
import ContactForm from './components/ContactForm.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    HeroSection,
    FeaturesSection,
    CtaSection,
    ContactForm,
    Footer
  }
}
</script>

<style>
/* Estilos específicos para App.vue */
main {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px 0;
}

/* Animações */
.fade-enter-active, .fade-leave-active {
  transition: opacity 0.5s;
}

.fade-enter, .fade-leave-to /* .fade-leave-active in <2.1.8 */ {
  opacity: 0;
}
</style>