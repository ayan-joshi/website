<script lang="ts">
	import { Main } from '$lib/layouts';
	import { DEFAULT_DESCRIPTION, DEFAULT_HOST } from '$lib/utils/metadata';
	import { TITLE_SUFFIX } from '$routes/titles';

	import FooterNav from '../../lib/components/FooterNav.svelte';
	import MainFooter from '../../lib/components/MainFooter.svelte';

	const title = 'Terms' + TITLE_SUFFIX;
	const description = DEFAULT_DESCRIPTION;
	const ogImage = DEFAULT_HOST + '/images/open-graph/website.png';
</script>

<svelte:head>
	<!-- Titles -->
	<title>{title}</title>
	<meta property="og:title" content={title} />
	<meta name="twitter:title" content={title} />
	<!-- Desscription -->
	<meta name="description" content={description} />
	<meta property="og:description" content={description} />
	<meta name="twitter:description" content={description} />
	<!-- Image -->
	<meta property="og:image" content={ogImage} />
	<meta property="og:image:width" content="1200" />
	<meta property="og:image:height" content="630" />
	<meta name="twitter:image" content={ogImage} />
	<meta name="twitter:card" content="summary_large_image" />
</svelte:head>

<Main>
	<div class="aw-container">
		<div class="aw-grid-120-1fr-auto" />

		<header class="aw-grid-120-1fr-auto-header">
			<h1 class="aw-title aw-u-color-text-primary">Terms and Conditions</h1>
		</header>

		<FooterNav />
		<MainFooter />
	</div>
</Main>
