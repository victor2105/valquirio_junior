<script>
	
	import { Nav, Footer } from '../components'

	export let segment;
</script>

<Nav {segment}/>

<slot></slot>

<Footer></Footer>
