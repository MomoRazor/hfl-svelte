<script module>
  import { defineMeta } from '@storybook/addon-svelte-csf';
  import Button from '../lib/Button.svelte' 

  const onNormalClick = () => {
    console.log('Normal Click!')
  }

  const onLoadClick = () => {
    console.log('Load Click!')
  }

  // More on how to set up stories at: https://storybook.js.org/docs/writing-stories
  const { Story } = defineMeta({
    title: 'Button',
    component: Button,
    tags: ['autodocs'],
    argTypes: {
      disabled: {
        control: 'boolean'
      },
      label: {
        control: 'text'
      },
      loading: {
        control: 'boolean'
      },
      variant: {
        control: { type: 'select' },
        options: [
          'primary',
          'secondary',
          'outlined'
        ]
      },
      size: {
        control: { type: 'select' },
        options: ['small', 'medium', 'large'],
      },
    },
    args: {
      onClick: onNormalClick,
      onLoadClick: onLoadClick
    }
  });
</script>

<Story name="Basic" args={{ label: 'Button' }} />
