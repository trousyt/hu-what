<template>
    <div v-bind:style="itemStyle"
         v-on:click="play"
         class="play-item">
        <span class="play-caption">
            {{ caption }}
        </span>
        <div class="play-overlay">
        </div>
        <audio v-bind:src="audioSrc" 
               ref="audio" preload />
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
                this.$refs.audio.play();
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
        font-size: .8rem;
        background-color: rgba(0,0,0,.5);
    }

    .play-overlay {
        background-color: rgba(0, 0, 0, 0, .5);
        background-image: url(../assets/play-button.png);
        background-repeat: no-repeat;
        background-blend-mode: overlay;
        max-width: 100%;
        max-height: 100%;
    }
</style>