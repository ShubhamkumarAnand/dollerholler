<div class="grid min-h-screen grid-cols-12 gap-x-16 bg-whisper">
	<header class="col-span-3 bg-daisyBush text-center">
		<a href="/invoices">
			<img src="images/logo.svg" alt="The Doller Holler Logo" class="mx-auto" />
		</a>
		<nav>
			<ul class="list-none text-2xl font-bold">
				<li>
					<a href="/invoices">Invoices</a>
				</li>
				<li><a href="/clients">Clients</a></li>
				<li><a href="#">setting</a></li>
				<li><a href="#">logout</a></li>
			</ul>
		</nav>
	</header>
	<main class="col-span-8 pt-10"><slot /></main>
</div>

<style lang="postcss">
	nav ul li {
		@apply mb-6;
	}
	nav ul li a {
		@apply font-bold text-white hover:text-goldenFizz;
	}
</style>
