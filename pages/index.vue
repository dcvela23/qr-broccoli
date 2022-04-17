<template>
    <div>

      <div class="container-fluid">
        <div class="row">
            <div class="col-sm-12 text-center" style="margin-top:30px; margin-bottom:50px;">
                <div class="h1">Hola oroz</div>
                <div class="h4">Eres:</div>
            </div>
        </div>
        <div class="row">
            <div class="container col-xs-12">
            <div class="col-sm-4 text-center">
                <div class="h3" style="margin-bottom:30px;">Guapo</div>
                <div class="w-300 h-300 img-circle center-block" :style="`background: url(require('~/assets/img_avatar3.png')); background-size: cover; background-position: center;`">
                  <img style="width: 100%" src="~/assets/1.png" />
                </div>
            </div>
            <div class="col-sm-4 text-center">
                <div class="h3" style="margin-bottom:30px;">Bello</div>
                <div class="w-300 h-300 img-circle center-block" :style="`background: url(require('~/assets/img_avatar3.png')); background-size: cover; background-position: center;`">
                  <img style="width: 100%" src="~/assets/2.png" />
                </div>
            </div>
            <div class="col-sm-4 text-center">
                <div class="h3" style="margin-bottom:30px;">Formidable</div>
                  <div class="w-300 h-300 img-circle center-block" :style="`background: url(require('~/assets/img_avatar3.png')); background-size: cover; background-position: center;`">
                    <img style="width: 100%" src="~/assets/3.png" />
                  </div>
                </div>
            </div>
        </div>
      </div>
  </div>
</template>
<script>
export default {
  computed: {
      homeData(){
        return this.$store.getters.getHomeData
      }
  },
}
</script>
<style scoped>
    .h1{
        color: #131982;
    }
    .h4{
        font-size: 20px;
        color: #666;
    }
    .h3{
        color: #666;
    }
    .p{
        font-family: 'Roboto,sans-serif';
        font-size: 15px;
        line-height: 2;
        color: #666;
    }
    .img-circle {
        border-radius: 50%;
    }
    .h-300 {
        height: 300px;
    }
    .w-300 {
        width: 300px;
    }

</style>
