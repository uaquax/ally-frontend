<script lang="ts">
  import "../global.css";
</script>

<svelte:head>
  <title>Ally</title>
</svelte:head>

<main>
  <h1>Welcome to Ally!</h1>
  <div class="links">
    <div class="sign-up">
      <a href="/signup"><button>Sign Up</button></a>
    </div>
    <div class="sign-in">
      <a href="/signin"><button>Sign In</button></a>
    </div>
  </div>
</main>

<style>
  @import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap");

  main {
    font-family: "Montserrat", sans-serif;

    width: 100vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #24292e;
    color: #eee;
    flex-direction: column;
  }

  .links {
    display: flex;
    gap: 0.5rem;
    flex-direction: row;
  }

  a {
    outline: none;
    text-decoration: none;
    color: #eee;
  }

  .sign-up button {
    margin-top: 20px;
    border: none;
    background-color: #455384;
    color: #eee;
    border-radius: 15px;
    width: 150px;
    height: 50px;
    padding: 10px;

    transition: all 0.1s ease;
  }

  .sign-up button:hover {
    background: none;

    box-shadow: 0px 0px 20px 4px #455384;
  }

  .sign-in button {
    margin-top: 20px;
    border: solid 1px #455384;
    background: none;
    color: #eee;
    border-radius: 15px;
    width: 150px;
    height: 50px;
    padding: 10px;

    transition: all 0.1s ease;
  }

  .sign-in button:hover {
    background-color: #455384;

    box-shadow: 0px 0px 20px 4px #455384;
  }
</style>
