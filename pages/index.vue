<template>
  <div>
    <h1>i78s.me</h1>

    <section>
      <h2><a href="https://github.com/i78s" target="_blank">GitHub</a></h2>
      <ul>
        <li>
          <a href="https://github.com/i78s/ValidateJS">https://github.com/i78s/ValidateJS</a>
        </li>
        <li>
          <a href="https://github.com/i78s/frontend-utils">https://github.com/i78s/frontend-utils</a>
        </li>
      </ul>
    </section>

    <section>
      <h2>Slides</h2>

      <p>社内向け勉強会の資料</p>

      <ul class="row">
        <li
          v-for="item in slides"
          class="col-lg-4"
        >
          <div v-html="item" class="slideshare">
          </div>
        </li>
      </ul>
    </section>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        repo: [
          {
            repoURL: 'https://github.com/i78s/ValidateJS',
            demo: 'https://i78s.me/ValidateJS/'
          }
        ],
        slides: [
          `<iframe src="//www.slideshare.net/slideshow/embed_code/key/27eNa6UdkzPKRn" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" allowfullscreen></iframe>`,
          `<iframe src="//www.slideshare.net/slideshow/embed_code/key/3KaCaq71jQK9im" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" allowfullscreen></iframe>`,
          `<iframe src="//www.slideshare.net/slideshow/embed_code/key/FUlxCVqAw0YWwt" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" allowfullscreen></iframe>`,
          `<iframe src="//www.slideshare.net/slideshow/embed_code/key/yDGYtrhyA83Kew" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" allowfullscreen></iframe>`
        ]
      }
    }
  }
</script>
<style>
  .slideshare{
    position: relative;
    padding-bottom: 66.66%;
    margin-bottom: 10px;
  }

  iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
</style>
