<template>
    <div v-bind:style="itemStyle"
         v-on:click="play"
         class="play-item">
        <span class="play-caption">
            {{ caption }}
        </span>
        <!-- <img v-bind:src="imgSrc" 
             v-bind:title="caption"
             v-on:click="play" /> -->
    </div>
</template>

<script>
    export default {
        props: {
            caption: String,
            audioSrc: String,
            imgSrc: String
        },
        data: function() {
            return {
                isPlaying: false
            }
        },
        methods: {
            play: function() {
                let audio = new Audio(this.audioSrc);
                audio.play();
                // TODO (trparkin): display play icon
            }
        },
        computed: {
            itemStyle: function() {
                return {
                    'font-size': '1px',
                    'background-image': `url(${this.imgSrc})`
                }
            }
        }
    }
</script>   

<style scoped>
    .play-item {
        background-size: contain;
        background-repeat: no-repeat;
    }

    .play-caption {
        display: inline-block;
        margin: 10px 0 -10px 0;
        padding: 5px;
        text-overflow: ellipsis;
        color: white;
        font-size: 14px;
        background: rgba(0, 0, 0, .5);
    }
</style>