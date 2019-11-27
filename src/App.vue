<template>
  <div id="app">
    <Navigation />
    <Header />
    <Services />
    <Portfolio />
    <About />
    <Team />
    <Clients />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import Navigation from './components/Navigation.vue';
import Header from './components/Header.vue';
import Services from './components/Services.vue';
import Portfolio from './components/Portfolio.vue';
import About from './components/About.vue';
import Team from './components/Team.vue';
import Clients from './components/Clients.vue';
import Contact from './components/Contact';
import Footer from './components/Footer.vue';

export default {
  name: 'app',
  components: {
    Navigation,
    Header,
    Services,
    Portfolio,
    About,
    Team,
    Clients,
    Contact,
    Footer,
  }
}
</script>