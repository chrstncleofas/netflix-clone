<template>
  <footer class="footer">
    <p>Questions? Call 1-866-579-7172</p>
    <div class="footer-cols">
      <ul>
        <li><a href="#">FAQ</a></li>
        <li><a href="#">Investor Relations</a></li>
        <li><a href="#">Ways To Watch</a></li>
        <li><a href="#">Corporate Information</a></li>
        <li><a href="#">Netflix Originals</a></li>
      </ul>
      <ul>
        <li><a href="#">Help Center</a></li>
        <li><a href="#">Jobs</a></li>
        <li><a href="#">Terms Of Use</a></li>
        <li><a href="#">Contact Us</a></li>
      </ul>
      <ul>
        <li><a href="#">Account</a></li>
        <li><a href="#">Redeem Gift Cards</a></li>
        <li><a href="#">Privacy</a></li>
        <li><a href="#">Speed Test</a></li>
      </ul>
      <ul>
        <li><a href="#">Media Center</a></li>
        <li><a href="#">Buy Gift Cards</a></li>
        <li><a href="#">Cookie Preferences</a></li>
        <li><a href="#">Legal Notices</a></li>
      </ul>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
.footer {
  max-width: 70%;
  margin: 1rem auto;
  overflow: auto;
}

.footer,
.footer a {
  color: #999;
  font-size: 0.9rem;
}

.footer p {
  margin-bottom: 1.5rem;
}

.footer .footer-cols {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-gap: 2rem;
}

.footer li {
  line-height: 1.9;
}

.footer .lang-select {
  margin-top: 2rem;
  color: #999;
  background-color: #000;
  background-image: none;
  border: 1px solid #333;
  padding: 1rem 1.2rem;
  border-radius: 5px;
}

@media (max-width: 960px) {
  .footer .footer-cols {
    grid-template-columns: repeat(2, 1fr);
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