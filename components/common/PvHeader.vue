<template>
  <header class="header">
    <div class="header-top">
      <div class="container">
        <div class="header-left d-none d-sm-block">
          <div
            class="info-box info-box-icon-left text-primary justify-content-start p-0"
          >
            <i class="icon-shipping"></i>
            <div class="info-box-content">
              <h4 class="text-transform-none">
                FREE Express Shipping On Orders $99+
              </h4>
            </div>
          </div>
        </div>

        <div class="header-right header-dropdowns ml-0 ml-sm-auto w-sm-100">
          <div class="header-dropdown mr-auto mr-sm-3 mr-md-0">
            <span><i class="flag-pa flag"></i>Spa</span>

            <div class="header-menu">
              <ul>
                <li><i class="flag-pa flag mr-2"></i>Spa</li>
              </ul>
            </div>
          </div>

          <div class="header-dropdown dropdown-expanded d-none d-lg-block">
            <a href="javascript:;">Links</a>
            <div class="header-menu">
              <ul>
                <li><nuxt-link to="/pages/account">Mi Cuenta</nuxt-link></li>
                <li><nuxt-link to="/pages/cart">Carrito</nuxt-link></li>
                <li>
                  <nuxt-link to="/pages/login" class="login-link"
                    >Iniciar Sesión</nuxt-link
                  >
                </li>
              </ul>
            </div>
          </div>

          <div class="social-icons">
            <a
              href="http://facebook.com"
              target="_blank"
              class="social-icon social-facebook icon-facebook"
            ></a>
            <a
              href="http://twitter.com"
              target="_blank"
              class="social-icon social-twitter icon-twitter"
            ></a>
            <a
              href="http://instagram.com"
              target="_blank"
              class="social-icon social-instagram icon-instagram"
            ></a>
          </div>
        </div>
      </div>
    </div>

    <div class="header-middle sticky-header mobile-sticky">
      <div class="container">
        <div class="header-left col-lg-2 w-auto pl-0">
          <button
            class="mobile-menu-toggler text-dark mr-2"
            type="button"
            @click="showMobileMenu"
          >
            <i class="fas fa-bars"></i>
          </button>

          <nuxt-link to="/" class="logo">
            <img
              src="~/static/images/logo-black.png"
              class="w-100"
              width="101"
              height="40"
              alt="Porto Logo"
            />
          </nuxt-link>
        </div>

        <div class="header-right w-lg-max">
          <pv-header-search></pv-header-search>

          <a class="d-lg-block d-none" title="login" @click="openLoginModal">
            <div class="header-user">
              <i class="icon-user-2"></i>
              <div class="header-userinfo">
                <span>Bienvenido</span>
                <h4 class="mb-0">Mi Cuenta</h4>
              </div>
            </div>
          </a>

          <!-- <nuxt-link
            to="/pages/wishlist"
            class="header-icon position-relative"
            title="wishlist"
          >
            <i class="icon-wishlist-2"></i
            ><span class="wishlist-count badge-circle">{{
              wishList.length
            }}</span>
          </nuxt-link> -->

          <!-- <pv-cart-menu></pv-cart-menu> -->
        </div>
      </div>
    </div>

    <div class="header-bottom sticky-header d-none d-lg-flex desktop-sticky">
      <div class="container">
        <!-- <pv-main-menu></pv-main-menu> -->
      </div>
    </div>
  </header>
</template>

<script>
// import PvMainMenu from '~/components/common/partials/PvMainMenu'
// import PvCartMenu from '~/components/common/partials/PvCartMenu'
import PvHeaderSearch from '~/components/common/partials/PvHeaderSearch'
// import { mapGetters } from 'vuex'

export default {
  components: {
    // PvMainMenu,
    // PvCartMenu,
    PvHeaderSearch,
  },
  data: function () {
    return {
      isHome: {
        type: Boolean,
        default: true,
      },
    }
  },
  computed: {},
  mounted: function () {},
  destroyed: function () {},
  methods: {
    openLoginModal: function () {},
    showMobileMenu: function () {},
    showMobileSearch: function (e) {},
    mouseOverHandler: function (e) {},
    mouseLeaveHandler: function (e) {},
  },
}
</script>
