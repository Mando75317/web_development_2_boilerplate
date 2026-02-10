<template>
    <div
      v-for="stock in stocks"
      :key="stock.name"
      class="bg-white rounded-lg shadow-md p-4 border border-gray-200 hover:shadow-lg transition-shadow"
    >
      <div class="flex justify-between items-center">
        <StockInfo :stock="stock" />
        <StockPrice :stock="stock" />
      </div>
    </div>
</template>

<script setup>
    import StockInfo from '../../molecules/StockInfo/StockInfo.vue'
    import StockPrice from '../../molecules/StockPrice/StockPrice.vue'
</script>