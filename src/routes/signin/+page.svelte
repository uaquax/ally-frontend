<script lang="ts">
  import "../../global.css";

  export let form;

  async function handleSubmit(event: SubmitEvent) {}
</script>

<div class="form">
  <a id="back-link" href="/"><button id="back">Back</button></a>

  <h1>Sign In</h1>

  <form on:submit={handleSubmit}>
    <div class="form-item">
      <label for="email">Email<sup><small>*</small></sup></label>
      <input
        value={form?.email ?? ""}
        type="email"
        id="email"
        name="email"
        required
        placeholder="Enter your email.."
      />
    </div>
    <div class="form-item">
      <label for="password">Password<sup><small>*</small></sup></label>
      <input
        value={form?.password ?? ""}
        type="password"
        placeholder="Enter your password.."
        id="password"
        name="password"
        required
      />
    </div>
    <button type="submit">Sign Up</button>
  </form>
  <div class="sign-in-text">
    Don't have an account? <a href="/signup">Sign Up</a>
  </div>
</div>

<style lang="css">
  @import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap");

  #back {
    position: absolute;
    top: 0;
    left: 0;
    width: 4rem;
    margin: 10px;
  }

  #back-link {
    outline: none;
    text-decoration: none;
    color: #eee;
  }

  .sign-in-text {
    margin-top: 20px;
  }

  .sign-in-text a {
    outline: none;
    text-decoration: none;
    color: #eee;
    background-color: #455384;
    padding: 5px;
    transition: all 0.3s ease;
  }

  .sign-in-text a:hover {
    box-shadow: 0px 0px 5px 2px #455384;

    /* border-radius: 10px; */
  }

  h1 {
    margin-bottom: 20px;
  }
  .form {
    font-family: "Montserrat", sans-serif;
    width: 100vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    background: #24292e;
    color: #eee;
  }

  form {
    max-width: 400px;
    width: 100%;
    padding: 20px;
    box-shadow: 0 0 1px 4px #455384;
    background: #24292e;
    color: #eee;
    border-radius: 8px;
  }

  .form-item {
    margin-bottom: 20px;
  }

  label {
    display: block;
    margin-bottom: 5px;
    color: #eee;
  }

  input {
    background: #24292e;
    width: 100%;
    padding: 10px;
    border: 1px solid #ddd;
    border-radius: 4px;
    box-sizing: border-box; /* Ensures padding doesn't affect overall width */
    color: #eee;
    transition: all 0.2s ease;
  }

  input::placeholder {
    color: #eee;
  }

  input:focus {
    outline: none;
    border-color: #546396;
    box-shadow: 0px 0px 10px 4px #455384;
  }

  button {
    width: 100%;
    padding: 10px;
    background-color: #455384;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    transition: all 0.2s ease;
  }

  button:hover {
    box-shadow: 0px 0px 10px 4px #455384;
    width: 90%;
    margin-left: 5%;
  }
</style>
