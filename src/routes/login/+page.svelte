<script>
	import Header from "../Header.svelte";
    let email = "";
    let password = "";
    
    const handleLogin = () => {
        // Lógica do login
        console.log(`Logging in with ${email} and ${password}`);
    };
</script>

<Header />

<div class="container">
    <h1 class="text-center">Login</h1>
    <form on:submit|preventDefault={handleLogin}>
        <div class="mb-3">
            <label for="email" class="form-label">Email address</label>
            <input type="email" class="form-control" id="email" bind:value={email} required>
        </div>
        <div class="mb-3">
            <label for="password" class="form-label">Password</label>
            <input type="password" class="form-control" id="password" bind:value={password} required>
        </div>
        <button type="submit" class="btn btn-primary">Login</button>
    </form>
</div>

<h1>Login</h1>