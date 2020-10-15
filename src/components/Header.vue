<template>
  <header class="showcase">
    <div class="showcase-top">
      <img src="./img/logo.png" alt="" />
      <a href="#" class="btn btn-rounded">Sign In</a>
    </div>
    <div class="showcase-content">
      <h1>See what's next</h1>
      <p>Watch anywhere. Cancel Anytime</p>
      <a href="#" class="btn btn-xl"
        >Watch Free For 30 Days <i class="fas fa-chevron-right btn-icon"></i
      ></a>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
.showcase {
  width: 100%;
  height: 93vh;
  position: relative;
  background: url("./img/background.jpg") no-repeat center center/cover;
}

.showcase::after {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 1;
  background: rgba(0, 0, 0, 0.6);
  box-shadow: inset 120px 100px 250px #000000, inset -120px -100px 250px #000000;
}

.showcase-top {
  position: relative;
  z-index: 2;
  height: 90px;
}

.showcase-top img {
  width: 170px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  margin-left: 0;
}

.showcase-top a {
  position: absolute;
  top: 50%;
  right: 0;
  transform: translate(-50%, -50%);
}

.showcase-content {
  position: relative;
  z-index: 2;
  width: 65%;
  margin: auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  margin-top: 9rem;
}

.showcase-content h1 {
  font-weight: 700;
  font-size: 5.2rem;
  line-height: 1.1;
  margin: 0 0 2rem;
}

.showcase-content p {
  text-transform: uppercase;
  color: #fff;
  font-weight: 400;
  font-size: 1.9rem;
  line-height: 1.25;
  margin: 0 0 2rem;
}

@media (max-width: 700px) {
  .showcase::after {
    background: rgba(0, 0, 0, 0.6);
    box-shadow: inset 80px 80px 150px #000000, inset -80px -80px 150px #000000;
  }

  .showcase-content h1 {
    font-size: 2.5rem;
    line-height: 1;
  }

  .showcase-content p {
    font-size: 1rem;
  }

  .btn-xl {
    font-size: 1rem;
    padding: 1.2rem 1.6rem;
    text-transform: uppercase;
  }
}

@media (max-width: 960px) {
  .showcase {
    height: 100vh;
  }

  .showcase-top img {
    top: 30%;
    left: 5%;
    transform: translate(0);
  }

  .showcase-content h1 {
    font-size: 3.7rem;
    line-height: 1;
  }

  .showcase-content p {
    font-size: 1.5rem;
  }

   .btn-xl {
    font-size: 1rem;
    padding: 1.2rem 1.6rem;
    text-transform: uppercase;
  }

}

@media (max-height: 600px) {
  .showcase-content {
    margin-top: 3rem;
  }
}
</style>