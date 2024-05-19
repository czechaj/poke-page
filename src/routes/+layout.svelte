<script>
	import { goto } from '$app/navigation';
	import '../app.css';
</script>

<div class="bg-base-100 justify-between fixed top-0 left-0 right-0">
	<div class="navbar max-w-5xl mx-auto justify-between">
		<div>
			<a href="/" class="btn btn-ghost text-xl">PokePage</a>
			<a href="/user" class="btn btn-ghost">My Page</a>
		</div>
		<div>
			<button on:click={() => goto('/login')} class="btn btn-ghost">Login</button>
			<span class="text-white text-lg ml-2"> cze@mail.com </span>
			<button on:click={() => console.log('logout')} class="btn btn-ghost">Logout</button>
		</div>
	</div>
</div>

<slot />
