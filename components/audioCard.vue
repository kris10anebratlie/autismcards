<template>
    <img :src="`/visuals/${visual}.jpg`" @click="play" alt="Clickable Image" style="max-height: 100px;" />
  </template>
  
  <script>
  import { useSound } from '@vueuse/sound'
  
  export default {
    props: {
      visual: String,
      audio: String
    },
    setup(props) {
      const audioPath = '/audio/' + props.audio + '.mp3'
      const { play } = useSound(audioPath)
  
      return {
        play
      }
    },
  }
  </script>
  