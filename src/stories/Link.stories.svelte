<script module>
  import { defineMeta } from '@storybook/addon-svelte-csf';
  import Link from '../lib/basics/Link.svelte' 
  import Text from '../lib/basics/Text.svelte' 

  // More on how to set up stories at: https://storybook.js.org/docs/writing-stories
  const { Story } = defineMeta({
    title: 'Link',
    component: Link,
    tags: ['autodocs'],
    argTypes: {
      to: {
        control: 'text'
      },
    }
  });

</script>

{#snippet text()}<Text>This is a link</Text>{/snippet}

<Story name="Basic" args={{ children: text }} />
