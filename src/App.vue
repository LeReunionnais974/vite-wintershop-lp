<script setup>
import Header from "./components/Header.vue";
import Nav from "./components/Nav.vue";
import Section from "./components/Section.vue";
import ForHer from "./components/home/ForHer.vue";
import Hero from "./components/home/Hero.vue";
import ForHim from "./components/home/ForHim.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
  <Nav />
  <Header />
  <Section>
    <ForHer />
  </Section>
  <Section>
    <Hero />
  </Section>
  <Section>
    <ForHim />
  </Section>
  <Footer />
</template>
