<script>
  import { page } from "$app/stores"
</script>

<nav>
  <a href="/" class:current-page={$page.url.pathname == "/"}>Home</a>
  <a href="help" class:current-page={$page.url.pathname.includes("help")}>Help</a>
  <a href="contactUs" class:current-page={$page.url.pathname.includes("contactUs")}>Contact Us</a>
</nav>

<style>
  nav {
    display: flex;
    align-content: center;
    justify-content: space-around;
  }
  a {
    color: black;
    font-family: "DM Sans", sans-serif;
    font-size: 120%;
  }

  a:hover {
    text-decoration: underline;
    font-weight: bolder;
  }
  .current-page {
    text-decoration: underline;
    font-weight: bolder;
  }
</style>
