<template>
    <div>
        <div>
            <label for="data">Data </label>
            <input id="data" type="text" placeholder="Ingrese datos" v-model="data"/>
            <button @click="pushMethod">push</button>
            <button @click="popMethod">pop</button>
        </div>   
        <div v-for="(item, index) in items" :key="index">
            {{item.message}}
        </div>
    </div>
</template>

<script>
export default {
  name: "PushPop",
  data() {
    return {
      items: [],
      data: ""
    };
  },
  methods: {
    pushMethod: function() {
      console.log("se ejecuto push");
      this.items.push({ message: this.data });
    },
    popMethod: function() {
      console.log("se ejecuto pop");
      this.items.pop();
    }
  }
};
</script>

<style>
</style>
