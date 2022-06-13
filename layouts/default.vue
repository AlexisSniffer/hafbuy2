<template>
  <div>
    <div class="page-wrapper">
      <pv-header></pv-header>
      <nuxt></nuxt>
      <!-- <pv-footer></pv-footer> -->

      <!-- <div class="wishlist-popup">
        <div class="wishlist-popup-msg">Product added!</div>
      </div> -->
    </div>

    <!-- <pv-cart-popup class="minipopup-area"></pv-cart-popup> -->

    <!-- <a
      id="scroll-top"
      href="javascript:;"
      title="Top"
      role="button"
      @click="scrollToTop"
    >
      <i class="icon-angle-up"></i>
    </a> -->

    <!-- <pv-mobile-menu></pv-mobile-menu> -->

    <!-- <pv-sticky-footer></pv-sticky-footer> -->
  </div>
</template>

<script>
import PvHeader from '~/components/common/PvHeader'
// import PvFooter from '~/components/common/PvFooter'
// import PvCartPopup from '~/components/common/partials/PvCartPopup'
// import PvMobileMenu from '~/components/common/partials/PvMobileMenu'
// import PvStickyFooter from '~/components/common/partials/PvStickyFooter'
/* import {
  // scrollTop,
  // stickyHeaderHandler,
  // resizeHandler,
  // showScrollTopHandler,
  // setCookie,
  // getCookie,
} from '~/utils' */

export default {
  components: {
    PvHeader,
    // PvFooter,
    // PvCartPopup,
    // PvMobileMenu,
    // PvStickyFooter,
  },
}
</script>
