<template>
    <div class="play-grid">
        <PlayItem v-for="item in playItems"
                  v-bind:key="item.audioSrc"
                  v-bind="item"
                  class="play-item" />
    </div>
</template>

<script>
    import PlayItem from './PlayItem.vue';

    export default {
        props: {
            playItems: Array
        },
        components: {
            PlayItem
        }
    }
</script>

<style>
    .play-grid {
        display: flex;
        flex-flow: row wrap;
    }

    .play-item {
        flex-grow: 1;
        height: 125px;
        width: 200px;
        max-width: 200px;
        margin-right: 10px;
    }

    .play-item img {
        max-height: 100px;
    }
</style>