# svelte-tailwindcss-breakpoint

A simple breakpoint helper for SvelteKit and TailwindCSS web apps.

## Install the package

```bash
npm i --save-dev @accuser/breakpoint
```

## Example

Add Breakpoint to the root layout to display the breakpoint helper in development mode.

```svelte
<script>
  import { Breakpoint } from '@accuser/breakpoint';
</script>

<Breakpoint />

<slot />
```
