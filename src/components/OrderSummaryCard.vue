<template>
  <div class='card'>
    <div class='card__header'>

    </div>
    <div class='card__body'>
      <h1>Order Summary</h1>
      <p>You can now listen to millions of songs, audiobooks, and podcasts on any device anywere you
        like!
      </p>
      <div class='plan'>
        <div class='plan__icon'>
          <icon-music />
        </div>
        <div class='plan__fee'>
          <p class='title'>
            Annual Plan
          </p>
          <p class='price'>
            $59.99/year
          </p>
        </div>
        <div class='plan__link'>
          <a href='#'>Change</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import IconMusic from '@/components/icons/IconMusic.vue';

export default {
  components: { IconMusic },
  props: {}
};
</script>

