<script>
	import logo from '$lib/images/svelte-logo.svg';

  const currentPath = window.location.href
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<main>
    <div class="">
      <img src={logo} alt="SvelteKit" class="logo" width="125" height="125" />
    </div>
    <div class="container">
      <div className="inner-container">
        <h2 class="header">
          You’ve just ignited a new
          <span class="library">Svelte</span> static site!
        </h2>
          <a href={currentPath}>
        <span class="pathname">
          {currentPath}
        </span>
          </a>
      </div>
      <p class="footer">Made in Nigeria with 💖</p>
    </div>
  </main>
</section>

<style>
main {
  height: 100vh;
  width: 100%;
  display: flex;
  flex-direction: column;
  gap: 7px;
  align-items: center;
  justify-content: center;
  border: 1px solid #eaeaea;
}
.logo {
  width: 200px;
  height: 200px;
}
.container {
  display: flex;
  flex-direction: column;
  text-align: center;
  gap: 25px;
}
.inner-container {
  display: flex;
  flex-direction: column;
  gap: 10px;
}
.header {
  font-size: 36px;
  font-weight: 400;
  color: #344054;
}
.pathname {
  color: #004eeb;
  font-size: 20px;
}
.footer {
  font-size: 20px;
  font-weight: 500;
  color: #344054;
}
.library {
  color: #FF3E00;
  font-weight: 600;
}
</style>



