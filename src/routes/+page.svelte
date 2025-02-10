<script lang="ts">
	import Link from "$lib/basics/Link.svelte";
    import Text from "$lib/basics/Text.svelte";
</script>


<div class='main'>
    <div class="center-text">
        <Text variant="h1">Welcome to the Human First Labs (HFL) Svelte Package</Text>
        <Text variant="h4">This package houses all the svelte code used in HFL projects, that is generic enough to be useful for different projects.</Text>
        <Text>All components here are mobile first, and designed with accessibility and performance in mind.</Text>
        <Text>You're free to use these components for your own projects, and if you haven't heard of HFL before, please <Link to="">check us out</Link>. Our stuff should look familiar ;).</Text>
        <!-- <Text>As with all Human First Labs projects, this is a non-profit endeavour, and so donations are vital and appreciated!</Text> -->
    </div>
    <div class="dependecy-list">
        <Text variant="h5">Dependancies:</Text>
        <ul>
            <li>
                <Text>unplugin-icons</Text>
            </li>
        </ul>
    </div>
</div>

<style>
    .main{
        flex-direction: column;
        background-color: var(--secondary-contrast-color);
        padding: 20px;
        border-radius: 20px;
    }

    .center-text{
        text-align: center;
        width: fit-content;
    }
</style>