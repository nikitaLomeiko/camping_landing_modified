<template>
  <!-- Navigation -->
  <Navigation logo="images/logo/agency-logo-small.png" label="*Foxy* Template" />

  <!-- Content Display -->
  <router-view />

  <!-- Footer -->
  <Footer>
    <FooterBlock :darken="false" :row="true">
      <FooterColumn
        title="О нас"
        faIcon="fa-solid fa-pen-to-square me-1 d-none d-md-inline"
        :description="[
          `This template is maintained by Ryan Balieiro and is based on the <a href='https://getbootstrap.com/'>Bootstrap</a> framework and the <a href='https://vuejs.org/'>Vue</a> framework.`,
        ]"
        :links="[]"
        :displayLinksAsButtons="false"
      />

      <FooterColumn
        title="Уютный кэмпинг для всей семьи"
        faIcon=""
        :description="[]"
        :links="[]"
        :displayLinksAsButtons="true"
      />

      <FooterColumn
        title="Связь"
        faIcon="fa fa-fax me-2"
        :description="[`999 Vue Developer's Avenue, 4A Suite 32`, `Cupertino – CA 01235`]"
        :links="[
          { label: `(555) 555-1234`, href: `tel:123456789`, faIcon: 'fa-regular fa-bell' },
          { label: `contact@foxyagency.com`, href: `mailto:foxy@agency.com`, faIcon: 'fa-regular fa-envelope' },
        ]"
        :displayLinksAsButtons="false"
      />
    </FooterBlock>

    <FooterBlock :darken="true" :row="false">
      <FooterCopyright
        holder="Ryan Balieiro"
        url="https://github.com/ryanbalieiro"
        license="Distributed Under the MIT License"
      />
    </FooterBlock>
  </Footer>
</template>

<script setup>
import Navigation from "/src/vue/components/nav/Navigation.vue";
import Footer from "/src/vue/components/footer/Footer.vue";
import FooterBlock from "/src/vue/components/footer/FooterBlock.vue";
import FooterCopyright from "/src/vue/components/footer/FooterCopyright.vue";
import FooterColumn from "/src/vue/components/footer/FooterColumn.vue";
</script>

<style lang="scss" scoped>
@import "/src/scss/_theming.scss";
</style>
