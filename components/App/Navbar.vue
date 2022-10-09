<template>
  <SfHeader
    :logo="shopLogo"
    :title="shopName"
    active-icon="account"
    searchPlaceholder="Mau cari apa?"
  >
    <template #navigation>
      <SfHeaderNavigationItem
        v-for="(category, key) in navbarLinks"
        :key="`sf-header-navigation-item-${key}`"
        :link="`${category.link}`"
        :label="category.title"
      />
    </template>
  </SfHeader>
</template>
<script>
import { SfHeader } from "@storefront-ui/vue";
export default {
  name: "Default",
  components: {
    SfHeader,
  },
  data() {
    return {
      shopName: "VSM COk",
      shopLogo: "/logo-jadi-01.svg",
      navbarLinks: [
        {
          title: "Cowok",
          link: "/",
        },
        {
          title: "Cewek",
          link: "/",
        },
      ],
    };
  },
};
</script>
