<script>
	let showMenu = false;

	function toggleNavbar() {
		showMenu = !showMenu;
	}
</script>

<nav class="bg-gray-800">
	<div class="max-w-6xl mx-auto">
		<div class="flex justify-between">
			<div class="flex space-x-4 py-5 px-2">
				<div class="mr-4">
					<a href="/" class="flex items-center">
						<svg
							xmlns="http://www.w3.org/2000/svg"
							fill="none"
							viewBox="0 0 24 24"
							stroke-width="1.5"
							stroke="currentColor"
							class="w-6 h-6 text-blue-600"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M12 12.75c1.148 0 2.278.08 3.383.237 1.037.146 1.866.966 1.866 2.013 0 3.728-2.35 6.75-5.25 6.75S6.75 18.728 6.75 15c0-1.046.83-1.867 1.866-2.013A24.204 24.204 0 0112 12.75zm0 0c2.883 0 5.647.508 8.207 1.44a23.91 23.91 0 01-1.152 6.06M12 12.75c-2.883 0-5.647.508-8.208 1.44.125 2.104.52 4.136 1.153 6.06M12 12.75a2.25 2.25 0 002.248-2.354M12 12.75a2.25 2.25 0 01-2.248-2.354M12 8.25c.995 0 1.971-.08 2.922-.236.403-.066.74-.358.795-.762a3.778 3.778 0 00-.399-2.25M12 8.25c-.995 0-1.97-.08-2.922-.236-.402-.066-.74-.358-.795-.762a3.734 3.734 0 01.4-2.253M12 8.25a2.25 2.25 0 00-2.248 2.146M12 8.25a2.25 2.25 0 012.248 2.146M8.683 5a6.032 6.032 0 01-1.155-1.002c.07-.63.27-1.222.574-1.747m.581 2.749A3.75 3.75 0 0115.318 5m0 0c.427-.283.815-.62 1.155-.999a4.471 4.471 0 00-.575-1.752M4.921 6a24.048 24.048 0 00-.392 3.314c1.668.546 3.416.914 5.223 1.082M19.08 6c.205 1.08.337 2.187.392 3.314a23.882 23.882 0 01-5.223 1.082"
							/>
						</svg>
						<span class="ml-2 text-2xl text-white">Logo</span>
					</a>
				</div>
				<!-- primary nav-->
				<div class="hidden items-center space-x-3 md:flex">
					<a href="/" class="text-white hover:text-blue-500">Dashboard</a>
					<a href="/" class="text-white hover:text-blue-500">Item1</a>
					<a href="/" class="text-white hover:text-blue-500">Item2</a>
				</div>
			</div>
			<!-- secondary nav-->
			<div class="hidden md:flex items-center space-x-4 mr-4">
				<a href="/" class="text-white hover:text-blue-500">Login</a>
				<a href="/" class="text-white hover:bg-blue-800 bg-blue-500 py-2 px-2 rounded translate duration-100"
					>Sign Up</a
				>
			</div>

			<!-- mobile button goes here -->
			<div class="md:hidden flex items-center mr-4">
				<button on:click={toggleNavbar} >
					<svg
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						class="w-6 h-6"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
						/>
					</svg>
				</button>
			</div>

		</div>
	</div>
	<!-- mobile menu -->
	<div
		class='md:hidden flex-col space-y-1 md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0 {showMenu
			? 'flex'
			: 'hidden'}'
	>
		<a href="/" class="block text-sm text-white hover:text-blue-500 hover:bg-gray-700 py-2 px-4">Dashboard</a>
		<a href="/" class="block text-sm text-white hover:text-blue-500 hover:bg-gray-700 py-2 px-4">Item1</a>
		<a href="/" class="block text-sm text-white hover:text-blue-500 hover:bg-gray-700 py-2 px-4">Item2</a>
		<div class="flex items-center text-white hover:text-blue-500 hover:bg-gray-700 px-3">
			<svg
				xmlns="http://www.w3.org/2000/svg"
				fill="none"
				viewBox="0 0 24 24"
				stroke-width="1.5"
				stroke="currentColor"
				class="w-6 h-6 "
			>
				<path
					stroke-linecap="round"
					stroke-linejoin="round"
					d="M15.75 9V5.25A2.25 2.25 0 0013.5 3h-6a2.25 2.25 0 00-2.25 2.25v13.5A2.25 2.25 0 007.5 21h6a2.25 2.25 0 002.25-2.25V15m3 0l3-3m0 0l-3-3m3 3H9"
				/>
			</svg>
			<a href="/" class="block text-sm py-2 px-1">Login</a>
		</div>
	</div>
</nav>

