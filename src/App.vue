<script setup>
  import configs from "./config.json"

  const models = configs.models
  const thumbnails = configs.thumbnails
  const max_epoc = configs.max_epoc
  const epoc_step_count = configs.epoc_step_count
</script>

<template>
  <p>
    <ul>
      <li v-for="model in models" :key="model.id">
        {{model.name}}
      </li>
    </ul>
    <br>
    <ul>
      <li v-for="thumbnail in thumbnails" :key="thumbnail.id">
        {{thumbnail.name}}
      </li>
    </ul>
    <br>
    Max Epocs: {{max_epoc}}
    <br>
    Epoc Step Count: {{epoc_step_count}}
    <br>
    <br>
    <ul>
      <li v-for="model in configs.models" :key="model.id">
        {{model.name}}
      </li>
    </ul>
    <br>
    <ul>
      <li v-for="thumbnail in configs.thumbnails" :key="thumbnail.id">
        {{thumbnail.name}}
      </li>
    </ul>
    <br>
    Max Epocs: {{configs.max_epoc}}
    <br>
    Epoc Step Count: {{configs.epoc_step_count}}
    <br>
  </p>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
