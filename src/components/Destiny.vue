<script setup>

function clickedYes() {
  alert("Yay! I'm so happy!");
}

function clickedNo() {
  alert("Oh no! I'm so sad!");
}
</script>

<template>
  <section>
    <div class="main">
      <div class="question">
        <h2 class="question">Do you want to go out with me?</h2>
      </div>

      <div class="buttons">
        <div>
          <button class="button-56" role="button" @click="clickedYes">Yes</button>
        </div>
        <div>
          <button class="button-56" role="button" @click="clickedNo">No</button>
        </div>
      </div>
    </div>
  </section>
</template>

<style>
.main {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  font-size: 2rem;
  margin: 100px;
}

.question {
  color: #111;
  text-shadow: 2px 2px 5px rgb(20, 18, 18);
}

.buttons {
  display: flex;
  flex-direction: row;
}

.button-56 {
  align-items: center;
  background-color: #fee6e3;
  border: 2px solid #111;
  border-radius: 8px;
  box-sizing: border-box;
  color: #111;
  cursor: pointer;
  display: flex;
  font-family: Inter, sans-serif;
  font-size: 16px;
  height: 48px;
  justify-content: center;
  line-height: 24px;
  max-width: 100%;
  padding: 0 25px;
  margin: 10px;
  position: relative;
  text-align: center;
  text-decoration: none;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
}

.button-56:after {
  background-color: #111;
  border-radius: 8px;
  content: "";
  display: block;
  height: 48px;
  left: 0;
  width: 100%;
  position: absolute;
  top: -2px;
  transform: translate(8px, 8px);
  transition: transform .2s ease-out;
  z-index: -1;
}

.button-56:hover:after {
  transform: translate(0, 0);
}

.button-56:active {
  background-color: #ffdeda;
  outline: 0;
}

.button-56:hover {
  outline: 0;
}

@media (min-width: 768px) {
  .button-56 {
    padding: 0 40px;
  }
}
</style>