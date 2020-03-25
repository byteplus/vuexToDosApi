<template>
    <div>
        Filter Dotos
        <select @change="filterTodos($event)">
            <option value="all">All</option>
            <option value="100">100</option>
            <option value="50">50</option>
            <option value="20">20</option>
            <option value="12">12</option>
        </select>
    </div>
</template>

<script>
import { mapActions } from "vuex";
    export default {
    name: "FilterTodos",
    methods: mapActions(["filterTodos"])
    };
</script>

<style scoped>
select {
  margin-top: 20px;
  padding: 6px;
  border: #41b883 1px solid;
}
</style>