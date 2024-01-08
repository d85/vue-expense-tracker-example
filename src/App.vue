<template>
  <TheHeader />
  <div class="container">
    <TheBalance />
    <IncomeExpenses />
    <TransactionList :transactions="transactions"/>
    <AddTransaction />
  </div>
</template>

<script setup>
import TheHeader from './components/TheHeader.vue'
import TheBalance from './components/TheBalance.vue'
import IncomeExpenses from './components/IncomeExpenses.vue'
import TransactionList from './components/TransactionList.vue'
import AddTransaction from './components/AddTransaction.vue'

import { ref } from 'vue'

const transactions = ref([
  { id: 1, text: 'Flower', amount: -19.99 },
  { id: 2, text: 'Salary', amount: 299.97 },
  { id: 3, text: 'Book', amount: -10 },
  { id: 4, text: 'Camera', amount: 150 },
])
</script>