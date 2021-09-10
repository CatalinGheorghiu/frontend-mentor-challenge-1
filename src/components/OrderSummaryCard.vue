<template>
  <section class='card'>
    <header class='card__header'>
      <img alt='' src='../assets/images/illustration-hero.svg'>
    </header>

    <main class='card__body'>
      <h1 class='title'>
        {{ bodyTitle }}
      </h1>
      <p class='description'>
        {{ bodyDescription }}
      </p>
      <div class='plan'>
        <div class='left-container'>
          <div class='plan__icon'>
            <icon-music />
          </div>
          <div class='plan__fee'>
            <p class='title'>
              {{ planFeeTitle }}
            </p>
            <p class='price'>
              {{ planFeePrice }}
            </p>
          </div>
        </div>
        <div class='plan__link'>
          <a href='#'>
            {{ planLink }}
          </a>
        </div>
      </div>
    </main>
    <footer class='card__footer'>
      <button class='btn btn--primary'>Proceed to Payment</button>
      <button class='btn btn--secondary'>Cancel Order</button>
    </footer>
  </section>
</template>

<script>
import IconMusic from '@/components/icons/IconMusic.vue';

export default {
  components: { IconMusic },
  props: {
    bodyTitle: {
      type: String,
      default: ''
    },
    bodyDescription: {
      type: String,
      default: ''
    },
    planFeeTitle: {
      type: String,
      default: ''
    },
    planFeePrice: {
      type: String,
      default: ''
    },
    planLink: {
      type: String,
      default: ''
    }
  }
};
</script>

