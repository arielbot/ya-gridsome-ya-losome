<template>
  <div>
    <header class="header">
      <div class="header-links">
        <strong>
          <g-link class="nav-link" to="/">{{ $static.metadata.siteName }}</g-link>
        </strong>
        <nav class="nav">
          <g-link class="nav-link" to="/">Home</g-link>
          <!--/* <g-link class="nav__link" to="/about/">About</g-link> */-->
        </nav>
      </div>
    </header>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>
.header {
  margin-bottom: 20px;
  border-bottom: 2px solid #000;
}
.header-links {
  max-width: 760px;
  margin: 20px auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.nav-link {
  margin: 0 20px;
  color: #18ac4c;
  text-transform: uppercase;
  text-decoration: none;
}
.nav-link:hover {
  text-decoration: underline;
}
</style>