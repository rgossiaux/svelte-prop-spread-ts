* Clone the repo
* `npm install`
* `npm run check`

## Expected

TypeScript errors:
* This component passes a function to `<Parent>`'s `name` prop, and also passes an `animal` prop https://github.com/rgossiaux/svelte-prop-spread-ts/blob/cbd721a3072aeaf5552178890c39de514200687e/src/routes/index.svelte#L9
* `<Parent>` spreads its props to `<Child>`: https://github.com/rgossiaux/svelte-prop-spread-ts/blob/057a71cfad1c3fb5024412076a20234780d4802d/src/lib/Parent.svelte#L5
* `<Child>` expects a `string` for `name`, and does not have an `animal` prop: https://github.com/rgossiaux/svelte-prop-spread-ts/blob/057a71cfad1c3fb5024412076a20234780d4802d/src/lib/Child.svelte#L2

Both the wrongly-typed `name` and the extra prop `animal` should throw type errors.

## Actual

No errors
