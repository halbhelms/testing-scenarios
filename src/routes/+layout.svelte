<nav>
  <a href="/">Home</a>
  <a href="/new">New</a>
  <a href="/scenarios">Scenarios</a>
</nav>

<slot />

<style>
  nav {
    display: flex;
    justify-content: space-around;
    padding: .2rem;
    margin-bottom: 1rem;
    background-color: #eee;
  }
  nav a {
    text-decoration: none;
    color: #333;
  }
  nav a:hover {
    text-decoration: underline;
  }

  :global(label) {
  display: inline-block;
  width: 200px;
  text-align: right;
  margin-left: 20px;
  margin-right: 6px;
}

:global(input) {
  width: 500px;
  border-radius: 4px;
  border: 1px solid lightgray;
  padding: 4px;
}

:global(main) {
  margin-bottom: 1rem;
  margin-left: 0;
}

</style>