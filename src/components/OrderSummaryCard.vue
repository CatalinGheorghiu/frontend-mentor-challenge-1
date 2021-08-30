<template>
  <div class='card'>
    <div class='card__header'>
      <img alt='' src='../assets/images/illustration-hero.svg'>
    </div>
    <div class='card__body'>
      <h1 class='title'>
        {{ bodyTitle }}
      </h1>
      <p class='description'>
        {{ bodyDescription }}
      </p>
      <div class='plan'>
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
        <div class='plan__link'>
          <a href='#'>
            {{ planLink }}
          </a>
        </div>
      </div>
    </div>
    <div class='card__footer'>
      <button class='btn btn--primary'>Proceed to Payment</button>
      <button class='btn btn--secondary'>Cancel Order</button>
    </div>
  </div>
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

