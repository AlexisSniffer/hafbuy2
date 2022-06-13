<template>
  <nav class="main-nav w-100">
    <ul class="menu main-menu sf-arrows w-100">
      <li class="menu-item" :class="{ show: isDepart }">
        <a
          href="javascript:;"
          class="d-inline-flex align-items-center sf-with-ul text-white"
          @click.prevent="mmenuAddHandler"
        >
          <i class="custom-icon-toggle-menu d-inline-table"></i
          ><span>ALL DEPARTMENTS</span></a
        >
        <div class="menu-depart-overlay" @click.stop="mmenuRemoveHandler"></div>
        <div class="menu-depart" :class="{ opened: isDepart }">
          <ul class="menu menu-vertical sf-arrows d-block no-superfish">
            <li>
              <a href="javascript:;" class="sf-with-ul"
                ><i class="icon-category-fashion"></i>Fashion</a
              >

              <div class="megamenu megamenu-fixed-width megamenu-one">
                <div class="row">
                  <div class="col-lg-3 mb-1 pb-2">
                    <a href="javascript:;" class="nolink pl-0">WOMAN</a>
                    <ul class="submenu">
                      <li>
                        <nuxt-link to="/shop">Top & Blouses</nuxt-link>
                      </li>
                      <li>
                        <nuxt-link to="/shop">Accessories</nuxt-link>
                      </li>
                      <li>
                        <nuxt-link to="/shop">Dresses & Skirts</nuxt-link>
                      </li>
                      <li>
                        <nuxt-link to="/shop">Shoes & Boots</nuxt-link>
                      </li>
                    </ul>

                    <a href="javascript:;" class="nolink pl-0">JEWELLERY</a>
                    <ul class="submenu">
                      <li>
                        <nuxt-link to="/shop">Sweaters</nuxt-link>
                      </li>
                      <li>
                        <nuxt-link to="/shop">Heels & Sandals</nuxt-link>
                      </li>
                      <li>
                        <nuxt-link to="/shop">Jeans & Shorts</nuxt-link>
                      </li>
                    </ul>
                  </div>
                  <div class="col-lg-4">
                    <a href="javascript:;" class="nolink pl-0">MAN</a>
                    <ul class="submenu">
                      <li>
                        <nuxt-link to="/shop">Accessories</nuxt-link>
                      </li>
                      <li>
                        <nuxt-link to="/shop">Watch Fashion</nuxt-link>
                      </li>
                      <li>
                        <nuxt-link to="/shop">Tees, Knits & Polos</nuxt-link>
                      </li>
                      <li>
                        <nuxt-link to="/shop">KOKA</nuxt-link>
                      </li>
                    </ul>

                    <a href="javascript:;" class="nolink pl-0">KIDS FASHION</a>
                    <ul class="submenu">
                      <li>
                        <nuxt-link to="/shop">Casual Shoes</nuxt-link>
                      </li>
                      <li>
                        <nuxt-link to="/shop">Spring & Autumn</nuxt-link>
                      </li>
                      <li>
                        <nuxt-link to="/shop">Winter Sneakers</nuxt-link>
                      </li>
                    </ul>
                  </div>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </li>

      <li>
        <nuxt-link to="/">Home</nuxt-link>
      </li>

      <li class="float-right phone">
        <a href="javascript:;" class="d-flex align-items-center"
          ><i class="icon-phone-1"></i>1-800-234-5678</a
        >
      </li>
    </ul>
  </nav>
</template>
<script>
// import { mainMenu } from '~/utils/data/menu'
// import Api, { baseUrl } from '~/api'
// import PvSmallProduct from '~/components/features/product/PvSmallProduct'
// import PvCarousel from '~/components/features/PvCarousel'
// import PvProductFour from '~/components/features/product/PvProductFour'
// import { homeSidebarSlider } from '~/utils/data/carousel'

export default {
  components: {
    // PvCarousel,
    // PvSmallProduct,
    // PvProductFour,
  },
  data: function () {
    return {
      isDepart: false,
      homeSidebarSlider: null,
    }
  },
}
</script>
