<template>
  <div id="app">
    <Piio domain-key="demo"/>

    <div class="home">
      <h1>Piio images for Vue.js</h1>
      <h2>Image tag example</h2>
      <PiioElement path="https://secureservercdn.net/198.71.233.106/w4y.80f.myftpupload.com/wp-content/uploads/2020/02/backpack-desktop.jpg" tag="img">
      </PiioElement>
      <PiioElement path="https://secureservercdn.net/198.71.233.106/w4y.80f.myftpupload.com/wp-content/uploads/2020/02/backpack-desktop.jpg" tag="IMG">
      </PiioElement>
      <hr>
      <h2>Background example</h2>
      <PiioElement path="https://secureservercdn.net/198.71.233.106/w4y.80f.myftpupload.com/wp-content/uploads/2020/02/backpack-desktop.jpg" tag="div"
      style="min-height:400px; color: #ffc107;background-size:cover;background-position:center;background-repeat:no-repeat">
        <h1>Your website faster,your images sharper.</h1>
      </PiioElement>

      <hr>
      <h2>Picture tag with multiple sources example</h2>
      <picture>
        <PiioElement path="https://secureservercdn.net/198.71.233.106/w4y.80f.myftpupload.com/wp-content/uploads/2020/02/backpack-desktop.jpg" tag="source" media="(min-width:969px)">
        </PiioElement>
        <PiioElement path="https://secureservercdn.net/198.71.233.106/w4y.80f.myftpupload.com/wp-content/uploads/2020/02/backpack-mobile.jpg" tag="source" media="(max-width:969px)">
        </PiioElement>
        <PiioElement path="https://secureservercdn.net/198.71.233.106/w4y.80f.myftpupload.com/wp-content/uploads/2020/02/backpack-mobile.jpg" tag="img">
        </PiioElement>
      </picture>
    </div>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

img {
  max-width:100%
}
.home {
  width: 90%;
  margin: 0 auto;
}
</style>
