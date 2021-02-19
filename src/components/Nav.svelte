<script lang="ts">
	export let segment: string;
</script>

<style>	
	nav {
		/* border-bottom: 1px solid rgba(255,62,0,0.1); */
		font-weight: 300;
		padding: 0 1em;
	}

	ul {
		margin: 0;
		padding: 0;
	}

	/* clearfix */
	ul::after {
		content: '';
		display: block;
		clear: both;
	}

	li {
		display: block;
		float: left;
	}

	[aria-current] {
		position: relative;
		display: inline-block;
	}

	[aria-current]::after {
		position: absolute;
		content: '';
		width: calc(100% - 1em);
		height: 2px;
		background-color: rgb(255,62,0);
		display: block;
		bottom: -1px;
	}

	a {
		text-decoration: none;
		padding: 1em 0.5em;
		display: block;
	}
</style>
<header class="w-full px-8 text-gray-700 bg-white" >
	<div class="container flex flex-col flex-wrap items-center justify-between py-5 mx-auto md:flex-row max-w-7xl">
	  <div class="relative flex flex-col md:flex-row">
		  <a href="#_" class="flex items-center mb-5 font-medium text-gray-900 lg:w-auto lg:items-center lg:justify-center md:mb-0">
			  <span class="mx-auto text-xl font-black leading-none text-gray-900 select-none">FactorPage<span class="text-indigo-600">.</span></span>
		  </a>
		  <nav class="flex flex-wrap items-center mb-5 text-base md:mb-0 md:pl-8 md:ml-8 md:border-l md:border-gray-200">
			  <a href="." class="mr-5 font-medium leading-6 text-gray-600 hover:text-gray-900" aria-current="{segment === undefined ? 'page' : undefined}">Home</a>
			  <a href="about" class="mr-5 font-medium leading-6 text-gray-600 hover:text-gray-900" aria-current="{segment === 'about' ? 'page' : undefined}">About</a>
			  <a href="#_" class="mr-5 font-medium leading-6 text-gray-600 hover:text-gray-900">Features</a>
			  <a href="price" class="mr-5 font-medium leading-6 text-gray-600 hover:text-gray-900" aria-current="{segment === 'price' ? 'page' : undefined}" >Pricing</a>
			  <a href="blog" class="mr-5 font-medium leading-6 text-gray-600 hover:text-gray-900" rel=prefetch aria-current="{segment === 'blog' ? 'page' : undefined}">Blog</a>
		  </nav>
	  </div>
  
	  <div class="inline-flex items-center ml-5 space-x-6 lg:justify-end">
		  <a href="#" class="text-base font-medium leading-6 text-gray-600 whitespace-no-wrap transition duration-150 ease-in-out hover:text-gray-900">
			  Sign in
		  </a>
		  <span class="inline-flex rounded-md shadow-sm">
			  <a href="#" class="inline-flex items-center justify-center px-4 py-2 text-base font-medium leading-6 text-white whitespace-no-wrap transition duration-150 ease-in-out bg-indigo-600 border border-transparent rounded-md hover:bg-indigo-500 focus:outline-none focus:border-indigo-700 focus:shadow-outline-indigo active:bg-indigo-700">
				  Sign up
			  </a>
		  </span>
	  </div>
	</div>
  </header>
  
