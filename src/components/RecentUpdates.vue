<template>
  <div class="updates">
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
.updates {
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
.updates h6 {
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

@media screen and (max-width: 1100px) {
  .updates {
    padding: 3% 6%;
  }

  .heading {
    font-size: 1.25rem;
  }
  .updates h6 {
    font-size: 2rem;
  }
  .overlay {
    padding: 0 4% 5%;
  }
  .overlay p {
    font-size: 0.9rem;
  }
  .overlay h4 {
    font-size: 1.7rem;
    line-height: 1.2;
  }
}

@media screen and (max-width: 870px) {
  .heading {
    font-size: 1.05rem;
  }
  .updates h6 {
    font-size: 1.7rem;
  }
  .posts {
    gap: 5px;
  }
  .overlay p {
    font-size: 0.85rem;
    margin: 0.5% 0;
  }
  .overlay h4 {
    font-size: 1.5rem;
    line-height: 1.2;
  }
}

@media screen and (max-width: 750px) {
  .posts {
    margin: 3% 0;
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 150px 150px 150px 150px;
    grid-template-areas:
      "one two "
      "one three "
      "four three "
      "four five ";
  }

  .overlay p {
    font-size: 0.8rem;
  }
  .overlay h4 {
    overflow: hidden;
    text-overflow: ellipsis;
    display: -webkit-box;
    -webkit-line-clamp: 2;
    -webkit-box-orient: vertical;
    font-size: 1.3rem;
  }
}

@media screen and (max-width: 650px) {
  .heading {
    font-size: 0.95rem;
  }
  .updates h6 {
    font-size: 1.5rem;
  }
}

@media screen and (max-width: 560px) {
  .heading {
    font-size: 0.9rem;
    margin: 0;
    /* text-align: center; */
  }
  .updates h6 {
    font-size: 1.4rem;
    /* text-align: center; */
  }
  .overlay p {
    font-size: 0.75rem;
  }
  .overlay h4 {
    font-size: 1.2rem;
  }
}
</style>
