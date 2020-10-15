<template>
  <section class="tab-content">
    <div class="container">
      <!-- Tab Content 1 -->
      <div id="tab-1-content" class="tab-content-item show">
        <div class="tab-1-content-inner">
          <div>
            <p class="text-lg">
              If you decide Netflix isn't for you - no problem. No commitment.
              Cancel online anytime.
            </p>
            <a href="#" class="btn btn-lg">Watch Free For 30 Days</a>
          </div>
          <img src="./img/tab-content-1.png" alt="" />
        </div>
      </div>

      <!-- Tab Content 2 -->
      <div id="tab-2-content" class="tab-content-item">
        <div class="tab-2-content-top">
          <p class="text-lg">
            Watch TV shows and movies anytime, anywhere — personalized for you.
          </p>
          <a href="#" class="btn btn-lg">Watch Free For 30 Days</a>
        </div>
        <div class="tab-2-content-bottom">
          <div>
            <img src="./img/tab-content-2-1.png" alt="" />
            <p class="text-md">Watch on your TV</p>
            <p class="text-dark">
              Smart TVs, PlayStation, Xbox, Chromecast, Apple TV, Blu-ray
              players and more.
            </p>
          </div>
          <div>
            <img src="./img/tab-content-2-2.png" alt="" />
            <p class="text-md">Watch instantly or download for later</p>
            <p class="text-dark">
              Available on phone and tablet, wherever you go.
            </p>
          </div>
          <div>
            <img src="./img/tab-content-2-3.png" alt="" />
            <p class="text-md">Use any computer</p>
            <p class="text-dark">Watch right on Netflix.com.</p>
          </div>
        </div>
      </div>

      <!-- Tab Content 3 -->
      <div id="tab-3-content" class="tab-content-item">
        <div class="text-center">
          <p class="text-lg">
            Choose one plan and watch everything on Netflix.
          </p>
          <a href="#" class="btn btn-lg">Watch Free For 30 Days</a>
        </div>

        <table class="table">
          <thead>
            <tr>
              <th></th>
              <th>Basic</th>
              <th>Standard</th>
              <th>Premium</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Monthly price after free month ends on 6/19/19</td>
              <td>$8.99</td>
              <td>$12.99</td>
              <td>$15.99</td>
            </tr>
            <tr>
              <td>HD Available</td>
              <td><i class="fas fa-times"></i></td>
              <td><i class="fas fa-check"></i></td>
              <td><i class="fas fa-check"></i></td>
            </tr>
            <tr>
              <td>Ultra HD Available</td>
              <td><i class="fas fa-times"></i></td>
              <td><i class="fas fa-times"></i></td>
              <td><i class="fas fa-check"></i></td>
            </tr>
            <tr>
              <td>Screens you can watch on at the same time</td>
              <td>1</td>
              <td>2</td>
              <td>4</td>
            </tr>
            <tr>
              <td>Watch on your laptop, TV, phone and tablet</td>
              <td><i class="fas fa-check"></i></td>
              <td><i class="fas fa-check"></i></td>
              <td><i class="fas fa-check"></i></td>
            </tr>
            <tr>
              <td>Unlimited movies and TV shows</td>
              <td><i class="fas fa-check"></i></td>
              <td><i class="fas fa-check"></i></td>
              <td><i class="fas fa-check"></i></td>
            </tr>
            <tr>
              <td>Cancel anytime</td>
              <td><i class="fas fa-check"></i></td>
              <td><i class="fas fa-check"></i></td>
              <td><i class="fas fa-check"></i></td>
            </tr>
            <tr>
              <td>First month free</td>
              <td><i class="fas fa-check"></i></td>
              <td><i class="fas fa-check"></i></td>
              <td><i class="fas fa-check"></i></td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "TabOne",
};
</script>

<style scoped>
/* Tab Content */
.tab-content {
  padding: 3rem 0;
  background: #000;
  color: #fff;
}

/* Hide initial content */
#tab-1-content,
#tab-2-content,
#tab-3-content {
  display: none;
  opacity: 0;
}

#tab-1-content .tab-1-content-inner {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-gap: 2rem;
  align-items: center;
  justify-content: center;
}

#tab-2-content .tab-2-content-top {
  display: grid;
  grid-template-columns: 2fr 1fr;
  grid-gap: 1rem;
  justify-content: center;
  align-items: center;
}

#tab-2-content .tab-2-content-bottom {
  margin-top: 2rem;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 2rem;
  text-align: center;
}

.table {
  width: 100%;
  margin-top: 2rem;
  border-collapse: collapse;
  border-spacing: 0;
}

.table thead th {
  text-transform: uppercase;
  padding: 0.8rem;
}

.table tbody {
  display: table-row-group;
  vertical-align: middle;
  border-color: inherit;
}

.table tbody tr td {
  color: #999;
  padding: 0.8rem 1.2rem;
  text-align: center;
}

.table tbody tr td:first-child {
  text-align: left;
}

.table tbody tr:nth-child(odd) {
  background: #222;
}

@media (max-width: 700px) {

  #tab-1-content .tab-1-content-inner {
    grid-template-columns: 1fr;
    text-align: center;
  }

  #tab-2-content .tab-2-content-top {
    display: block;
    text-align: center;
  }

  #tab-2-content .tab-2-content-bottom {
    margin-top: 2rem;
    display: grid;
    grid-template-columns: 1fr;
    grid-gap: 2rem;
    text-align: center;
  }

}
</style>