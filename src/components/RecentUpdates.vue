<template>
  <div class="sponsors">
    <p class="heading">Recent Updates</p>
    <h6>Recent Updates from Lorem Ipsum</h6>
  </div>
  <div class="posts">
    <div class="post one">
      <img src="kukah.svg" />
      <div class="overlay">
        <p>Technology <span>13 Sept, 2021</span></p>
        <h4>The Kukah Innovation Prize and Awards</h4>
      </div>
    </div>
    <div class="post two">
      <img src="kukah.svg" />
      <div class="overlay">
        <p>Technology <span>13 Sept, 2021</span></p>
        <h4>The Kukah Innovation Prize and Awards</h4>
      </div>
    </div>
    <div class="post three">
      <img src="kukah.svg" />
      <div class="overlay">
        <p>Technology <span>13 Sept, 2021</span></p>
        <h4>The Kukah Innovation Prize and Awards</h4>
      </div>
    </div>
    <div class="post four">
      <img src="kukah.svg" />
      <div class="overlay">
        <p>Technology <span>13 Sept, 2021</span></p>
        <h4>The Kukah Innovation Prize and Awards</h4>
      </div>
    </div>
    <div class="post five">
      <img src="kukah.svg" />
      <div class="overlay">
        <p>Technology <span>13 Sept, 2021</span></p>
        <h4>The Kukah Innovation Prize and Awards</h4>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.sponsors {
  padding: 3% 10%;
}
p,
h4 {
  margin: 0;
}

.heading {
  margin: 1% 0;
  font-size: 1.5rem;
  font-weight: 400;
  color: #8d354a;
}
.sponsors h6 {
  font-weight: 900;
  font-size: 2.5rem;
}

.posts {
  margin: 3% 0;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 200px 200px 200px;
  gap: 10px;
  grid-template-areas:
    "one two three"
    "four two three"
    "four five three";
}

img {
  object-fit: cover;
  width: 100%;
  height: 100%;
  /* border-radius: 10px; */
}
.one {
  grid-area: one;
}
.four {
  grid-area: four;
}
.two {
  grid-area: two;
}
.three {
  grid-area: three;
}
.five {
  grid-area: five;
}

.post {
  position: relative;
}

.overlay {
  content: "";
  position: absolute;
  height: 100%;
  width: 100%;
  top: 0;
  left: 0;
  background: rgb(0, 0, 0, 0.6);
  color: white;
  display: flex;
  flex-direction: column;
  justify-content: end;
  padding: 0 4% 7%;
}

.overlay p {
  color: rgb(255, 255, 255, 0.9);
  font-size: 0.95rem;
}

.overlay h4 {
  font-weight: 900;
}

.overlay span {
  margin-left: 2%;
}
</style>
