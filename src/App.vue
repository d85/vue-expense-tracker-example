<template>
  <TheHeader />
  <div class="container">
    <TheBalance />
    <IncomeExpenses />
    <TransactionList />
    <AddTransaction />
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import TheBalance from './components/TheBalance.vue'
import IncomeExpenses from './components/IncomeExpenses.vue'
import TransactionList from './components/TransactionList.vue'
import AddTransaction from './components/AddTransaction.vue'

export default {
  components: {
    TheHeader,
    TheBalance,
    IncomeExpenses,
    TransactionList,
    AddTransaction
  }
}
</script>