<template>
  <div>
    <div class="row">
      <div class="col-md-12">
        <SfHero class="hero" :slider-options="{ autoplay: false }">
          <SfHeroItem
            v-for="(img, index) in heroes"
            :key="index"
            :title="img.title"
            :subtitle="img.subtitle"
            :button-text="img.buttonText"
            :background="img.background"
            :image="img.img"
            :class="img.className"
            :buttonText="img.cok"
          />
        </SfHero>
      </div>
      <div class="col-md-12">
        <h4 class="text-center mt-5 mb-5">All Products</h4>
      </div>
    </div>

    <div v-if="products.length">
      <div class="row mb-5">
        <ProductCard
          v-for="product in products"
          :key="product.id"
          :item="product"
        />
      </div>
    </div>
  </div>
</template>

<script>
import Axios from "axios";
import { SfHero } from "@storefront-ui/vue";
export default {
  name: "ProductsIndex",
  components: {
    SfHero,
  },
  data() {
    return {
      products: [],
      heroes: [
        {
          title: "VMS Merchandise",
          subtitle: "Koleksi Januari 2022",
          buttonText: "Learn more",
          background: "#FCE4EC",
          cok: "Pingin tahu?",
          img: "/mockup_logo_2.png",
        },
        {
          title: "VMS Merchandise",
          subtitle: "JUNE COLLECTION 2022",
          buttonText: "Learn more",
          background: "rgb(239, 235, 233)",
        },
        {
          title: "VMS Merchandise",
          subtitle: "JUNE COLLECTION 2022",
          buttonText: "Learn more",
          background: "rgb(236, 239, 241)",
        },
      ],
    };
  },
  async fetch() {
    // Fetching the products from Medusa server
    try {
      const {
        data: { products },
      } = await Axios.get(`${process.env.baseUrl}/store/products`);
      this.products = products;
    } catch (e) {
      console.log("An error occured", e);
    }
  },
};
</script>
