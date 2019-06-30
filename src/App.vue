<template>
  <div id="app">
    <PlayGrid v-bind:playItems="playItems" />
  </div>
</template>

<script>
import PlayGrid from './components/PlayGrid.vue'

export default {
  name: 'app',
  components: {
    PlayGrid
  },
  data: function() {
    return {
      playItems: [
        { 
          caption: 'I love you dad... Hu-what?',
          imgSrc: 'media/I-love-you-dad--hu-what.png',
          audioSrc: 'media/I-love-you-dad--hu-what.mp3',
        },
        {
          caption: 'Hu-what?',
          imgSrc: 'media/hu-what.png',
          audioSrc: 'media/hu-what.mp3'
        },
        { 
          caption: 'I love you... Hu-what?',
          imgSrc: 'media/I-love-you--Hu-what.png',
          audioSrc: 'media/I-love-you--Hu-what.mp3',
        },
        { 
          caption: 'I found myself saying that all the time...',
          imgSrc: 'media/I-found-myself-saying-it.png',
          audioSrc: 'media/I-found-myself-saying-it.mp3',
        },
        { 
          caption: 'My life changed... I stayed home mostly alone...',
          imgSrc: 'media/I-stayed-home.png',
          audioSrc: 'media/I-stayed-home.mp3',
        },
        { 
          caption: 'I... missed out on everything',
          imgSrc: 'media/I-missed-out-on-everything.png',
          audioSrc: 'media/I-missed-out-on-everything.mp3',
        },
        { 
          caption: 'I felt like that I had stopped living. It was aweful.',
          imgSrc: 'media/I-felt-like-I-had-stopped-living.png',
          audioSrc: 'media/I-felt-like-I-had-stopped-living.mp3',
        },
        { 
          caption: 'The cost was ridiculous',
          imgSrc: 'media/The-cost-was-ridiculous.png',
          audioSrc: 'media/The-cost-was-ridiculous.mp3',
        },
        { 
          caption: 'A state of the art TV only costs 6 or 700 dollars',
          imgSrc: 'media/State-of-the-art-TV.png',
          audioSrc: 'media/State-of-the-art-TV.mp3',
        },
        { 
          caption: 'But a tiny hearing aid costs 3000, 5000, whatever they can get',
          imgSrc: 'media/3000-5000-whatever-they-can-get.png',
          audioSrc: 'media/3000-5000-whatever-they-can-get.mp3',
        },
        { 
          caption: 'It\'s just ridiculous',
          imgSrc: 'media/Its-just-ridiculous.png',
          audioSrc: 'media/Its-just-ridiculous.mp3',
        },
        { 
          caption: 'Well not anymore',
          imgSrc: 'media/Well-not-anymore.png',
          audioSrc: 'media/Well-not-anymore.mp3',
        },
        { 
          caption: 'It\'s magnetic',
          imgSrc: 'media/Its-magnetic.png',
          audioSrc: 'media/Its-magnetic.mp3',
        },
        { 
          caption: 'They\'re FDA cleared',
          imgSrc: 'media/Theyre-FDA-cleared.png',
          audioSrc: 'media/Theyre-FDA-cleared.mp3',
        },
        { 
          caption: 'I really love my hearing aids',
          imgSrc: 'media/I-really-love-my-hearing-aids.png',
          audioSrc: 'media/I-really-love-my-hearing-aids.mp3',
        },
        { 
          caption: 'I said I love you',
          imgSrc: 'media/I-said-I-love-you.png',
          audioSrc: 'media/I-said-I-love-you.mp3',
        },
        { 
          caption: 'I heard you the first time, I just wanted to hear it again',
          imgSrc: 'media/I-heard-it-the-first-time.png',
          audioSrc: 'media/I-heard-it-the-first-time.mp3',
        },
      ]
    }
  }
}
</script>

<style>
body {
  margin: 0;
  padding: 0;
  font-size: 12px;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 1024px;
}
</style>
