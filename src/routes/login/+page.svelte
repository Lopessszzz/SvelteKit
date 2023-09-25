<script>
    import Header from "../Header.svelte";
    let username = '';
    let password = '';
    let agreement = false;
    
    function handleSubmit() {
      if (username && password && agreement) {
        alert(`Usuário: ${username}, Senha: ${password}`);
      }
    }
  </script>
  
  <Header />

  <style>
    .form-container {
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      background-color: #f5f5f5;
    }
    .form-signin {
      width: 100%;
      max-width: 330px;
      padding: 15px;
      margin: auto;
      background-color: #fff;
      border-radius: 5px;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    }
  </style>
  
  <div class="form-container">
    <form class="form-signin" on:submit|preventDefault={handleSubmit}>
      <img class="mb-4" src="https://getbootstrap.com/docs/5.3/assets/brand/bootstrap-logo.svg" alt="" width="72" height="72">
      <h1 class="h3 mb-3 fw-normal">Please sign in</h1>
  
      <div class="mb-3">
        <label for="username" class="visually-hidden">Nome do usuário</label>
        <!-- svelte-ignore a11y-autofocus -->
        <input type="text" class="form-control" id="username" bind:value={username} placeholder="Digite seu usuário" required autofocus>
      </div>
      
      <div class="mb-3">
        <label for="password" class="visually-hidden">Senha</label>
        <input type="password" class="form-control" id="password" bind:value={password} placeholder="Digite sua senha" required>
      </div>
  
      <div class="checkbox mb-3">
        <label>
          <input type="checkbox" id="agreement" bind:checked={agreement} required> Concordo com os termos
        </label>
      </div>
      <button class="w-100 btn btn-lg btn-primary" type="submit" disabled={!username || !password || !agreement}>Sign in</button>
      <p class="mt-5 mb-3 text-muted">&copy; 2022</p>
    </form>
  </div>

<h1>Login</h1>

