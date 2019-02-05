<template>
    <div class="container">
        <div class="row">
            <div class="col-md-8 col-md-offset-2">
                <div class="panel panel-default">
                    <div class="panel-heading">Example Component</div>

                    <div class="panel-body">
                        {{getNumber}}
                    </div>
                    <!-- <plyr-youtube :id="youtubeID" :pe="false" /> -->
                    <!-- youtube div element -->
<!-- youtube div element -->
<vue-plyr>
  <div data-plyr-provider="youtube" data-plyr-embed-id="bTqVqk7FSmY"></div>
</vue-plyr>
<h1>Ok...</h1>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
window.addEventListener('resize', function() {
  if (!document.fullscreenElement) {
    return;
  }

  var minimumScreenSize = 0.33;
  var screenArea = screen.width * screen.height;
  var windowArea = window.outerHeight * window.outerWidth;

  // If the size of the window relative to the screen is less than a third,
  // let's assume we're in PiP and exit fullscreen to prevent Auto PiP.
  if ((windowArea / screenArea) < minimumScreenSize) {
    document.exitFullscreen();
  }
});
    export default {
        
        mounted() {
            console.log('Component mounted.')
        },
        computed: {
            getNumber(){
                return this.$store.getters.getNumber;
            },
            youtubeID(){
                return 'zGhG5Y22dwY';
            }
        }
    }
</script>
