<template>
  <header class="header">
    <div class="container header__container">
      <div class="header__logo">
        <div class="header__logo-img"></div>
      </div>
      <nav>
        <ul class="header__menu">
          <li
            v-for="(item, index) in links"
            :key="index"
            :class="{ active: item.active }"
          >
            <a href="">{{ item.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data: function () {
    return {
      links: [
        {
          url: "#",
          text: "Characters",
          active: false,
        },
        {
          url: "#",
          text: "Comics",
          active: false,
        },
        {
          url: "#",
          text: "Movies",
          active: true,
        },
        {
          url: "#",
          text: "TV",
          active: false,
        },
        {
          url: "#",
          text: "Games",
          active: false,
        },
        {
          url: "#",
          text: "Collectibles",
          active: false,
        },
        {
          url: "#",
          text: "Videos",
          active: false,
        },
        {
          url: "#",
          text: "Fans",
          active: false,
        },
        {
          url: "#",
          text: "News",
          active: false,
        },
        {
          url: "#",
          text: "Shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.header {
  height: $header-height;
  &__container {
    display: flex;
  }
  &__logo {
    flex-grow: 1;
    padding: 1rem;
    .header__logo-img {
      height: 100%;
      background-image: url(../assets/img/dc-logo.png);
      background-repeat: no-repeat;
      background-position: left;
      background-size: contain;
    }
  }
  &__menu {
    display: flex;
    li {
      line-height: $header-height;
      padding: 0 0.5rem;
      &.active {
        border-bottom: 5px solid $brand-primary-color;
      }
      a {
        color: $text-darkgrey;
        &:hover {
          color: $brand-primary-color;
        }
      }
    }
  }
}
</style>
