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
