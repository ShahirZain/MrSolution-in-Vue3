<template>
  
  <div class="myWrapper container">
    <div class="flex flex-row">
      <div class="bg-opacity-10 mt-10 ml-20  mr-10  lg:block hidden">
        <ul>
          <li
            v-for="item in variant"
            :key="item"
            class="border border-opacity-25 border-blue-900 w-32 text-center py-1 hover:border-gray-500"
          >
            {{ item }}
          </li>
        </ul>
      </div>
      <div>
        <slider />
      </div>
    </div>
    <div class="lg:mx-20 mx-10 mt-10">
      <FashionProduct />
    </div>
  </div>
</template>

<script>
import slider from "../landingPage/slider/slider";
import FashionProduct from "./fashionProduct";

export default {
  name: "fashion",
  components: {
    slider,
    FashionProduct,
  },
  data() {
    return {
      variant: [
        "Linen",
        "Wool",
        "Cotton",
        "Linen",
        "Wool",
        "Cotton",
        "Linen",
        "Wool",
        "Cotton",
      ],
    };
  },
};
</script>
<style scoped>
.myWrapper.container{
  width:80%;
  margin:0 auto;
}
</style>