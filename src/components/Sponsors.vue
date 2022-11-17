<template>
  <div class="sponsors">
    <p>Our Clients And Partners</p>
    <h6>Some organisations we've loved working with</h6>

    <div class="sponsors_group">
      <div class="sponsor_item">
        <img src="sponsors/microsoft.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/kdsg.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/kadipa.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/agrolog.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/softalliance.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/kukah.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/cleantech.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/rabitz.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/bantu.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/certiport.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/ukaid.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/mastercard.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/dbi.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/itf.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/nbte.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/victoryxr.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/google.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/meta.svg" alt="" />
      </div>
      <div class="sponsor_item">
        <img src="sponsors/pan.svg" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.sponsors {
  padding: 3% 10%;
}
p,
h6 {
  margin: 0;
}

.sponsors p {
  margin: 1% 0;
  font-size: 1.5rem;
  font-weight: 400;
  color: #8d354a;
}
.sponsors h6 {
  font-weight: 900;
  font-size: 2.5rem;
}
.sponsors_group {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  margin: 4% 0;
  padding: 0 2%;
}
.sponsor_item {
  border: 1px solid grey;
  height: 25vh;
  display: grid;
  justify-content: center;
  place-items: center;
}

.sponsor_item img {
  width: 100%;
  object-fit: cover;
  filter: grayscale(100%);
  transition: 0.8s ease;
}
.sponsor_item:hover img {
  filter: none;
}
</style>
