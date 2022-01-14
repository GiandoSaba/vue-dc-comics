<template>
  <section class="card-section">
    <div class="container">
      <ul>
        <li>
          <img
            src="../assets/img/buy-comics-digital-comics.png"
            alt="Digital-Comics"
          />
          <a href="#">Digital Comics</a>
        </li>
        <li>
          <img
            src="../assets/img/buy-comics-merchandise.png"
            alt="Digital-Comics"
          />
          <a href="#">DC Merchandise</a>
        </li>
        <li>
          <img
            src="../assets/img/buy-comics-subscriptions.png"
            alt="Digital-Comics"
          />
          <a href="#">Subscriptions</a>
        </li>
        <li>
          <img
            src="../assets/img/buy-comics-shop-locator.png"
            alt="Digital-Comics"
          />
          <a href="#">Comic Shop Locator</a>
        </li>
        <li>
          <img src="../assets/img/buy-dc-power-visa.svg" alt="Digital-Comics" />
          <a href="#">DC Power Visa</a>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: "FooterCard",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/style.scss";

.card-section {
  background-color: $brand-font-color;
  padding: 2.5em;
  ul {
    @include flex(center, center);
    gap: 8px;
    li {
      @include flex(center, center);
      flex-basis: calc(100% / 5);
      img {
        height: 50px;
        margin-right: 1em;
      }
      a {
        text-transform: uppercase;
      }
    }
  }
}
</style>
