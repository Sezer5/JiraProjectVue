<template>
  <nav>
    <button @click="updateFilter('all')">Hepsi</button>
    <button @click="updateFilter('completed')">Tamamlananlar</button>
    <button @click="updateFilter('continue')">Devam Edenler</button>
  </nav>
</template>

<script>
export default {
    emits:['filterChange'],
    props:['current'],
    methods:{
        updateFilter(filterValue){
            this.$emit('filterChange',filterValue)
        }
    }
}
</script>

<style>

</style>