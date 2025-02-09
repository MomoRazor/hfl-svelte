<script module>
  import { defineMeta } from '@storybook/addon-svelte-csf';
  import Text from '../lib/Text.svelte' 

  // More on how to set up stories at: https://storybook.js.org/docs/writing-stories
  const { Story } = defineMeta({
    title: 'Text',
    component: Text,
    tags: ['autodocs'],
    argTypes: {
      variant: {
        control: 'select',
        options: [
          'h1', 'h2' , 'h3' ,'h4' ,'h5' ,'h6' , 'small' , 'p' , 'span'
        ]
      },
      children: {
        control: 'text'
      }
    },
  });
</script>

<Story name="Basic" args={{ children: 'This is some random text!' }} />
