<script module>
	import { defineMeta } from '@storybook/addon-svelte-csf';
	import Image from '../lib/Image.svelte';

	// More on how to set up stories at: https://storybook.js.org/docs/writing-stories
	const { Story } = defineMeta({
		title: 'Image',
		component: Image,
		tags: ['autodocs'],
		argTypes: {
			src: {
				control: 'text'
			},
			placeholderSrc: {
				control: 'text'
			},
			alt: {
				control: 'text'
			}
		}
	});
</script>

<Story name="Basic" />
