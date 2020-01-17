<template>
  <div class="hero-wrap">
    <div class="container">
      <div class="row">
        <div class="col-sm-6 col-xs-12 hero-text">
          <div class="card">
              <h3><b>Yoga</b> is the journey of the self, through the self, to the self</h3>
              <p>It is a long established fact that a reader will be distracted by the readable content of a page
              when looking at its layout. The point of using
              Lorem Ipsum.</p>
              <button class="btn btn-outline tosca">LEARN MORE</button>
          </div>
        </div>
        <div class=" col-sm-6 col-xs-12 hero-image">
          <img src="@/assets/images/heroimage.png">
        </div>
      </div>
    </div>

  </div>
</template>

<script>

export default {
  name: 'HeroImage'
}
</script>
<style lang="scss">
  .hero-wrap{
    padding: 30px 0;
    .hero-text {
        align-items: center;
        min-height: 45vh;
        display: flex;
        justify-content: center;
        text-align: left;
        .card {
          border: 0;
          display: block;
        }
    }
    .hero-image {
        text-align: right;
    }
  }

</style>