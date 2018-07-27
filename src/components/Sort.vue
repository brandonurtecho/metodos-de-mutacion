<template>
    <div>
        <div>
            <button @click="ascendingSortMethod">Ordenar ascendentemente</button>
            <button @click="descendingSortMethod">Ordenar descendentemente</button>
        </div>   
        <div v-for="(item, index) in items" :key="index">
            {{item}}
        </div>
    </div>    
</template>

<script>
export default {
  name: "Sort",
  data() {
    return {
      items: [3, 8, 1, 2, 7, 4, 9]
    };
  },
  methods: {
    ascendingSortMethod: function() {
      this.items.sort();
    },
    descendingSortMethod: function() {
      this.items.sort().reverse();
    }
  }
};
</script>

<style>
</style>
