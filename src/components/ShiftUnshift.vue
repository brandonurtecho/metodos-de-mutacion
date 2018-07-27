<template>
    <div>
        <div>
            <label for="data">Data </label>
            <input id="data" type="text" placeholder="Ingrese datos" v-model="data"/>
            <button @click="unshiftMethod">unshift</button>
            <button @click="shiftMethod">shift</button>
        </div>   
        <div v-for="(item, index) in items" :key="index">
            {{item.message}}
        </div>
    </div>        
</template>

<script>
export default {
  name: "Example",
  data() {
    return {
      items: [],
      data: ""
    };
  },
  methods: {
    unshiftMethod: function() {
      console.log("se ejecuto unshift");      
      this.items.unshift({ message: this.data });
    },
    shiftMethod: function() {
      console.log("se ejecuto shift");
      this.items.shift();
    }
  }
};
</script>

<style>
</style>
