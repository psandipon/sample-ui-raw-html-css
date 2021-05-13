<template>
  <div class="home">
    <header class="site-header">
      <a href="#0" class="logo" style="padding-right:100px"> <b>Logo</b></a>

      <nav class="site-nav">
        <ul>
          <li class="active"><a href="#0">1.HAIR</a></li>
          <li><a href="#0">2.SKIN</a></li>
          <li><a href="#0">1.SEX</a></li>
          <li><a href="#0">1.BLOG</a></li>
        </ul>
      </nav>

      <div class="actions">
        <nav class="site-nav">
          <ul>
            <li><a href="#0">search</a></li>
            <li><a href="#0">ENG </a></li>
            <li><a href="#0">ACCOUNT</a></li>
          </ul>
        </nav>
        <div class="circle"></div>
      </div>
    </header>
  </div>
</template>

<script>
export default {
  components: {},
};
</script>
<style lang="scss" scoped>
.site-header {
  background: #ffffff;
  color: white;
  display: flex;
  align-items: center;
  margin: 20px;
}

.logo {
  text-decoration: none;
  color: rgb(0, 0, 0);
  font-size: 1.5rem;
  text-transform: uppercase;
  padding: 10px;
}
.site-nav {
  ul {
    list-style: none;
    display: flex;
    margin: 0;
    padding: 0;
  }
  a {
    text-transform: uppercase;
    text-decoration: none;
    color: #cdd0d0;
    padding: 20px;
    display: inline-block;
  }
  .active {
    a {
      font-weight: bold;
      color: #484848;
    }
  }
}
.site-nav:hover {
  a:hover {
    font-weight: bold;
    color: #000000;
  }
}
.actions {
  margin-left: auto;
  display: flex;
  align-items: center;
  margin-right: 10px;
}

.circle {
  height: 35px;
  width: 35px;
  background-color: #555;
  border-radius: 50%;
  margin: 0;
}
</style>
