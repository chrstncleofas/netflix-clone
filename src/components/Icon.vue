<template>
  <section class="tabs">
    <div class="container">
      <div id="tab-1" class="tab-item tab-border">
        <i class="fas fa-door-open fa-3x"></i>
        <p class="hide-sm">Cancel at any time</p>
      </div>
      <div id="tab-2" class="tab-item">
        <i class="fas fa-tablet-alt fa-3x"></i>
        <p class="hide-sm">Watch anywhere</p>
      </div>
      <div id="tab-3" class="tab-item">
        <i class="fas fa-tags fa-3x"></i>
        <p class="hide-sm">Pick your price</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Tabs",
};
</script>

<style scoped>
.tabs {
  background: var(--dark-color);
  padding-top: 1rem;
  border-bottom: 3px solid #3d3d3d;
  border-right: none;
}

.tabs .container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 1rem;
  align-items: center;
  justify-content: center;
  text-align: center;
}

.tabs p {
  font-size: 1.2rem;
  padding-top: 0.5rem;
}

.tabs .container > div {
  padding: 1.5rem 0;
}

.tabs .container > div:hover {
  color: #fff;
  cursor: pointer;
}

.tab-border {
  border-bottom: var(--primary-color) 4px solid;
}

@media (max-width: 960px) {

  .hide-sm {
    display: none;
  }


  .btn-xl {
    font-size: 1.5rem;
    padding: 1.4rem 2rem;
    text-transform: uppercase;
  }

  .text-xl {
    font-size: 1.5rem;
  }

  .text-lg {
    font-size: 1.3rem;
    margin-bottom: 1rem;
  }

  .text-md {
    margin-bottom: 1rem;
    font-size: 1.2rem;
  }
}

</style>