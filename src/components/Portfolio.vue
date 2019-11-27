<template>
  <section class="bg-light page-section" id="portfolio">
    <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="section-heading text-uppercase">Portfolio</h2>
          <h3 class="section-subheading text-muted">Lorem ipsum dolor sit amet consectetur.</h3>
        </div>
      </div>
      <div class="row">
        <div class="col-md-4 col-sm-6 portfolio-item" v-for="(obj, key) in portfolioJSON" :key="key">
          <a class="portfolio-link" data-toggle="modal" href="#portfolioModal6">
            <div class="portfolio-hover">
              <div class="portfolio-hover-content">
                <i class="fas fa-plus fa-3x"></i>
              </div>
            </div>
            <img class="img-fluid" :src="obj.img" alt="asdasd">
          </a>
          <div class="portfolio-caption">
            <h4>{{obj.caption}}</h4>
            <p class="text-muted">{{obj.title}}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>

    import img1 from './../../src/assets/img/portfolio/01-thumbnail.jpg';
    import img2 from './../../src/assets/img/portfolio/02-thumbnail.jpg';
    import img3 from './../../src/assets/img/portfolio/03-thumbnail.jpg';
    import img4 from './../../src/assets/img/portfolio/04-thumbnail.jpg';
    import img5 from './../../src/assets/img/portfolio/05-thumbnail.jpg';
    import img6 from './../../src/assets/img/portfolio/06-thumbnail.jpg';


    export default {
        name: 'Portfolio',
        data: () => ({
            portfolioJSON: [
                {
                    img: img1,
                    caption: 'Threads',
                    title: 'Illustration',
                },
                {
                    img: img2,
                    caption: 'Explore',
                    title: 'Graphic Design',
                },
                {
                    img: img3,
                    caption: 'Finish',
                    title: 'Identity',
                },
                {
                    img: img4,
                    caption: 'Lines',
                    title: 'Branding',
                },
                {
                    img: img5,
                    caption: 'Southwest',
                    title: 'Website Design',
                },
                {
                    img: img6,
                    caption: 'Window',
                    title: 'Photography',
                },

            ]
        }),
    }
</script>
<style scoped>

</style>