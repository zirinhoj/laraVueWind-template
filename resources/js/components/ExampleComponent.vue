<template>
  <div>
    <div v-for="person in persons" :key="person.id">
      <h1 class="font-bold text-xl">name: {{ person.name }}</h1>
      <h3>age: {{ person.age }}</h3>
    </div>
    <div>
      <h1 class="text-lg">name: {{ people.name }}</h1>
      <h3>age: {{ people.age }}</h3>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return{
      persons: [
        {name: 'name 1', age: '1',},
        {name: 'name 2', age: '2',},
        {name: 'name 3', age: '3',},
        {name: 'name 4', age: '4',},
      ],
      people: {name: 'another name', age: '1'},
    }
  }
}
</script>

<style>

</style>