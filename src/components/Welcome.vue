<template>
  <div id="welcomeContainer">
    <div id="imgContainer">
      <img id="profileImage" src="/img/hairNGlasses.png" />
    </div>
    <span id="helloText" class="light-green--text px-auto display-2">&gt;Hi, I'm Dustin_</span>
  </div>
</template>

<script>
export default {};
</script>

<style>
#welcomeContainer {
  background-image: url("/img/computer1.jpg"),
    linear-gradient(
      180deg,
      white,
      white,
      white,
      white,
      white,
      white,
      white,
      white,
      white,
      gray,
      dimgray,
      black
    );
  background-blend-mode: multiply;
  background-size: cover;
  background-position: center;
  height: 100vh;
}

#imgContainer {
  padding-top: 80px;
}

#profileImage {
  max-width: 300px;
  text-align: center;
  display: block;
  margin: 0px auto 0px auto;
  background: url("/img/hairNGlassesOrig.png");
  background-size: contain;
  background-repeat: no-repeat;
  -webkit-filter: drop-shadow(1px 1px 2px rgba(0, 0, 0, 0.9))
    drop-shadow(1px -1px 2px #222) drop-shadow(-1px -1px 2px #222)
    drop-shadow(-1px 1px 2px #222);
  filter: drop-shadow(1px 1px 2px rgba(0, 0, 0, 0.2))
    drop-shadow(1px -1px 2px rgba(0, 0, 0, 0.2))
    drop-shadow(-1px -1px 2px rgba(0, 0, 0, 0.2))
    drop-shadow(-1px 1px 2px rgba(0, 0, 0, 0.2))
    drop-shadow(2px 2px 6px rgba(0, 0, 0, 0.1))
    drop-shadow(2px -2px 6px rgba(0, 0, 0, 0.1))
    drop-shadow(-2px -2px 6px rgba(0, 0, 0, 0.1))
    drop-shadow(-2px 2px 6px rgba(0, 0, 0, 0.1));
}
#helloText {
  text-shadow: -1px -1px 2px #000, 1px -1px 2px #000, -1px 1px 2px #000,
    2px 1px 2px #000, -2px -2px 4px #000, 2px -2px 4px #000, -2px 2px 4px #000,
    2px 2px 4px #000;
  width: 100vw;
  text-align: center;
  display: block;
  padding-top: 20px;
}
</style>