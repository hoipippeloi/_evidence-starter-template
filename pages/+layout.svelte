<script>
	import '../app.css';
	import { EvidenceDefaultLayout } from '@evidence-dev/core-components';
	export let data;

	import "$lib/uikit-3.17.11/css/uikit.min.css";
	import "$lib/uikit-3.17.11/js/uikit.min.js";
	import "$lib/uikit-3.17.11/js/uikit-icons.min.js";
	import "$lib/css/style.css";

	import NavMenu from "$lib/ui/NavMenu.svelte";
</script>

<svelte:head>
	<title>Evidence starter template</title>
</svelte:head>

<EvidenceDefaultLayout {data} 
  	title='My App'
  	neverShowQueries=true
  	githubRepo='https://github.com/hoipippeloi/_evidence-starter-template'
  	hideSidebar=true
  	fullWidth=true
  	maxWidth=1440
  >
  
  <NavMenu {data} />
  <slot slot="content" />

</EvidenceDefaultLayout>
