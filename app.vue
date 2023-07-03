<template>
  <div class="text-center">
    <h1 class="text-4xl font-inter">Welcome to MyApp</h1>
    <h2 class="text-lg text-gray-600">Building Amazing Web Applications</h2>
  </div>
  <div class="card-grid">
    <div v-for="card in cards" :key="card.audio">
      <AudioCard :audio="card.audio" :visual="card.visual" class="card" />
    </div>
  </div>
</template>

<script>

export default {
  data() {
    return {
      cards: [
        {
          visual: 'sleepy',
          audio: 'trombone'
        },
        {
          visual: 'sleepy copy',
          audio: 'trombone'
        },
        {
          visual: 'sleepy',
          audio: 'trombone'
        },
        {
          visual: 'sleepy copy',
          audio: 'trombone'
        },
        {
          visual: 'sleepy',
          audio: 'trombone'
        },
        {
          visual: 'sleepy copy',
          audio: 'trombone'
        },
        {
          visual: 'sleepy',
          audio: 'trombone'
        },
        {
          visual: 'sleepy copy',
          audio: 'trombone'
        },
        {
          visual: 'sleepy',
          audio: 'trombone'
        },
        {
          visual: 'sleepy copy',
          audio: 'trombone'
        },
        {
          visual: 'sleepy',
          audio: 'trombone'
        },
        {
          visual: 'sleepy copy',
          audio: 'trombone'
        },
        {
          visual: 'sleepy',
          audio: 'trombone'
        },
        {
          visual: 'sleepy copy',
          audio: 'trombone'
        }
      ]
    }
  }
}
</script>

<style scoped>
.card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  grid-gap: 10px;
}

.card {
  background-color: #f2f2f2;
  padding: 10px;
}
</style>