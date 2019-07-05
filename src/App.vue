<template>
  <div id="app">
    <PlayGrid v-bind:playItems="playItems" />
  </div>
</template>

<script>
import PlayGrid from './components/PlayGrid.vue';

export default {
  name: 'app',
  components: {
    PlayGrid
  },
  data: function() {
    return {
      playItems: [
        { 
          caption: 'I love you dad',
          imgSrc: 'media/I-love-you-dad.png',
          audioSrc: 'media/I-love-you-dad.mp3',
        },
        {
          caption: 'Hu-what?',
          imgSrc: 'media/hu-what.png',
          audioSrc: 'media/hu-what.mp3'
        },
        { 
          caption: 'I love you',
          imgSrc: 'media/I-love-you.png',
          audioSrc: 'media/I-love-you.mp3',
        },
        { 
          caption: 'Hu-what (background)',
          imgSrc: 'media/Hu-what--background.png',
          audioSrc: 'media/Hu-what--background.mp3',
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
          caption: 'I felt like that I had stopped living',
          imgSrc: 'media/I-felt-like-I-had-stopped-living.png',
          audioSrc: 'media/I-felt-like-I-had-stopped-living.mp3',
        },
        { 
          caption: 'It was aweful',
          imgSrc: 'media/it-was-aweful.png',
          audioSrc: 'media/it-was-aweful.mp3',
        },
        { 
          caption: 'I knew I needed hearing aids',
          imgSrc: 'media/I-knew-I-needed-hearing-aids.png',
          audioSrc: 'media/I-knew-I-needed-hearing-aids.mp3',
        },
        { 
          caption: 'The cost was ridiculous',
          imgSrc: 'media/The-cost-was-ridiculous.png',
          audioSrc: 'media/The-cost-was-ridiculous.mp3',
        },
        { 
          caption: 'A tiny hearing aid',
          imgSrc: 'media/A-tiny-hearing-aid.png',
          audioSrc: 'media/A-tiny-hearing-aid.mp3',
        },
        { 
          caption: 'A state of the art TV only costs 6 or 700 dollars',
          imgSrc: 'media/State-of-the-art-TV.png',
          audioSrc: 'media/State-of-the-art-TV.mp3',
        },
        { 
          caption: 'A tiny hearing aid costs 3000, 5000',
          imgSrc: 'media/3000-5000-whatever-they-can-get.png',
          audioSrc: 'media/3000-5000-whatever-they-can-get.mp3',
        },
        { 
          caption: 'Whatever they can get',
          imgSrc: 'media/whatever-they-can-get.png',
          audioSrc: 'media/whatever-they-can-get.mp3',
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
          caption: 'My life is so much better',
          imgSrc: 'media/My-life-is-so-much-better.png',
          audioSrc: 'media/My-life-is-so-much-better.mp3',
        },
        { 
          caption: 'Rechargeable, state of the art digital hearing aids',
          imgSrc: 'media/State-of-the-art-hearing-aids.png',
          audioSrc: 'media/State-of-the-art-hearing-aids.mp3',
        },
        {
          caption: 'You can\'t see them',
          imgSrc: 'media/You-cant-see-them.png',
          audioSrc: 'media/You-cant-see-them.mp3'
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
          caption: 'I like them',
          imgSrc: 'media/I-like-them.png',
          audioSrc: 'media/I-like-them.mp3'
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
          caption: 'I heard you the first time',
          imgSrc: 'media/I-heard-you-the-first-time.png',
          audioSrc: 'media/I-heard-you-the-first-time.mp3',
        },
        { 
          caption: 'I just wanted to hear it again',
          imgSrc: 'media/I-just-wanted-to-hear-it-again.png',
          audioSrc: 'media/I-just-wanted-to-hear-it-again.mp3',
        },
        { 
          caption: 'If you need hearing aids',
          imgSrc: 'media/If-you-need-hearing-aids.png',
          audioSrc: 'media/If-you-need-hearing-aids.mp3',
        },
        { 
          caption: 'Tired of changing batteries',
          imgSrc: 'media/Tired-of-changing-batteries.png',
          audioSrc: 'media/Tired-of-changing-batteries.mp3',
        },
        { 
          caption: 'Hearing Assist will change your life',
          imgSrc: 'media/Hearing-Assist-will-change-your-life.png',
          audioSrc: 'media/Hearing-Assist-will-change-your-life.mp3',
        },
        { 
          caption: 'You can buy two',
          imgSrc: 'media/you-can-buy-two.png',
          audioSrc: 'media/you-can-buy-two.mp3',
        },
        { 
          caption: 'Visit hearing assist dot com',
          imgSrc: 'media/visit-hearing-assist-dot-com.png',
          audioSrc: 'media/visit-hearing-assist-dot-com.mp3',
        },
        { 
          caption: 'Gift the gift of hearing to someone you love',
          imgSrc: 'media/give-the-gift-of-hearing.png',
          audioSrc: 'media/give-the-gift-of-hearing.mp3',
        },
        { 
          caption: 'Two two, two two',
          imgSrc: 'media/two-two-two-two.png',
          audioSrc: 'media/two-two-two-two.mp3',
        },
      ]
    }
  }
}
</script>

<style lang='scss'>
@import "./assets/app.scss";

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
