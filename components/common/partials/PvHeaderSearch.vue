<template>
  <div
    class="header-icon header-search header-search-inline header-search-category w-lg-max text-right mb-0 d-none d-sm-block"
  >
    <a class="search-toggle" role="button" @click.stop="searchToggle">
      <i class="icon-search-3"></i>
    </a>

    <form
      action="#"
      method="get"
      @click.stop="showSearchForm"
      @submit.prevent="submitSearchForm"
    >
      <div class="header-search-wrapper">
        <label for="search_term" class="sr-only">Buscar</label>
        <input
          :id="'search_term' + getId"
          v-model="search_term"
          type="text"
          class="form-control"
          name="search_term"
          placeholder="Buscar..."
          required
          @input="searchProducts"
        />
        <div class="select-custom">
          <select v-model="searchCategory" @change="searchProducts">
            <option value>All Categories</option>
            <option value="fashion">Fashion</option>
            <option value="women">- Women</option>
            <option value="men">- Men</option>
            <option value="jewellery">- Jewellery</option>
            <option value="kids">- Kids Fashion</option>
            <option value="electronics">Electronics</option>
            <option value="smart-tvs">- Smart TVs</option>
            <option value="cameras">- Cameras</option>
            <option value="games">- Games</option>
            <option value="home-garden">Home &amp; Garden</option>
            <option value="motors">Motors</option>
            <option value="cars-and-trucks">- Cars and Trucks</option>
            <option value="motorcycles-powersports">
              - Motorcycles &amp; Powersports
            </option>
            <option value="accessories">- Parts &amp; Accessories</option>
            <option value="boats">- Boats</option>
            <option value="supplies">- Auto Tools &amp; Supplies</option>
          </select>
        </div>
        <button
          class="btn icon-magnifier p-0"
          title="search"
          type="submit"
        ></button>
      </div>
    </form>
  </div>
</template>
<script>
export default {
  data: function () {
    return {
      search_term: '',
      suggestions: [],
      timeouts: [],
      searchCategory: '',
    }
  },

  computed: {
    getId: function () {
      return Math.random() * 100
    },
  },

  mounted: function () {},

  methods: {
    searchProducts: function () {},
    searchToggle: function (e) {},
    showSearchForm: function (e) {},
    closeSearchForm: function (e) {},
    submitSearchForm: function (e) {},
    handler(e) {},
  },
}
</script>
