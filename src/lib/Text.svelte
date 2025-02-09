<script lang="ts">

  interface Props {
    /** This is the text tag to be used here*/
    variant?: 'h1' | 'h2' | 'h3' | 'h4' | 'h5' | 'h6' | 'small' | 'p' | 'span'
    /** This is just the text */
    children: string
  }
  
  const { variant ="p", children }: Props = $props();
</script>

<svelte:element this={variant} class={[
    'basic-text',
]}>{children}</svelte:element>

<style>
  .basic-text {
    display: inline-block;
    line-height: 1;
    font-family: var(--general-font);
  }
</style>