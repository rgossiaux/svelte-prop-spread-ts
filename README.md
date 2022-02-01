* Clone the repo
* `npm install`
* `npm run check`

## Expected

A TypeScript error:
* This component passes a function to `<Parent>`'s `name` prop https://github.com/rgossiaux/svelte-prop-spread-ts/blob/057a71cfad1c3fb5024412076a20234780d4802d/src/routes/index.svelte#L9
* `<Parent>` spreads its props to `<Child>`: https://github.com/rgossiaux/svelte-prop-spread-ts/blob/057a71cfad1c3fb5024412076a20234780d4802d/src/lib/Parent.svelte#L5
* `<Child>` expects a `string` for `name`: https://github.com/rgossiaux/svelte-prop-spread-ts/blob/057a71cfad1c3fb5024412076a20234780d4802d/src/lib/Child.svelte#L2

## Actual

No error
