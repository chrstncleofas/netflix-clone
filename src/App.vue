<template>
  <div id="app">
    <Header />
    <Icon />
    <Tab />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header";
import Icon from "./components/Icon";
import Tab from "./components/Tab";
import Footer from "./components/Footer";

export default {
  name: "App",
  components: {
    Header,
    Icon,
    Tab,
    Footer,
  },
};
</script>

<style>

:root {
  --primary-color: #e50914;
  --dark-color: #141414;
  --light-color: #f4f4f4;
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: "Arial", sans-serif;
  -webkit-font-smoothing: antialiased;
  background: #000;
  color: #999;
}

ul {
  list-style: none;
}

h1,
h2,
h3,
h4 {
  color: #fff;
}

a {
  color: #fff;
  text-decoration: none;
}

p {
  margin: 0.5rem 0;
}

img {
  width: 100%;
}

/* Container */
.container {
  max-width: 70%;
  margin: auto;
  overflow: hidden;
  padding: 0 2rem;
}

/* Text Styles */
.text-xl {
  font-size: 2rem;
}

.text-lg {
  font-size: 1.8rem;
  margin-bottom: 1rem;
}

.text-md {
  margin-bottom: 1.5rem;
  font-size: 1.2rem;
}

.text-center {
  text-align: center;
}

.text-dark {
  color: #999;
}

/* Buttons */
.btn {
  display: inline-block;
  background: var(--primary-color);
  color: #fff;
  padding: 0.4rem 1.3rem;
  font-size: 1rem;
  text-align: center;
  border: none;
  cursor: pointer;
  margin-right: 0.5rem;
  transition: opacity 0.2s ease-in;
  outline: none;
  box-shadow: 0 1px 0 rgba(0, 0, 0, 0.45);
  border-radius: 2px;
}

.btn:hover {
  opacity: 0.9;
}

.btn-rounded {
  border-radius: 5px;
}

.btn-xl {
  font-size: 2rem;
  padding: 1.5rem 2.1rem;
  text-transform: uppercase;
}

.btn-lg {
  font-size: 1rem;
  padding: 0.8rem 1.3rem;
  text-transform: uppercase;
}

.btn-icon {
  margin-left: 1rem;
}

.show {
  display: block !important;
  opacity: 1 !important;
  transition: all 1000 ease-in;
}


</style>
