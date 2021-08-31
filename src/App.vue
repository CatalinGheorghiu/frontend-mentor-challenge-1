<template>
  <div id='app'>
    <OrderSummaryCard
      body-description='
        You can now listen to millions of songs, audiobooks, and podcasts on
        any device anywere you
        like!'
      body-title='Order Summary'
      plan-fee-price='$59.99/year'
      plan-fee-title='Annual Plan'
      plan-link='Change' />
  </div>
</template>

<script>
import OrderSummaryCard from './components/OrderSummaryCard.vue';

export default {
  name: 'App',
  components: {
    OrderSummaryCard
  }
};
</script>

