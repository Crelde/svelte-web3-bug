# Bug reproduction for [svelte-web3](https://github.com/clbrge/svelte-web3)

When using latest web3js:

```html
<script src="https://cdn.jsdelivr.net/npm/web3@latest/dist/web3.min.js"></script>
```

We are getting this error when trying to use MetaMask browser provider:

```
Uncaught (in promise) s: Web3 validator found 1 error[s]:
value "1337" at "/0" must pass "hex" validation
    at c.validate (https://cdn.jsdelivr.net/npm/web3@latest/dist/web3.min.js:2:634195)
    at t.Web3Validator.validate (https://cdn.jsdelivr.net/npm/web3@latest/dist/web3.min.js:2:636887)
    at t.hexToNumber (https://cdn.jsdelivr.net/npm/web3@latest/dist/web3.min.js:2:589899)
    at alwaysNumber (http://127.0.0.1:5174/node_modules/.vite/deps/svelte-web3.js?v=d385d017:17695:60)
    at switch1193Provider (http://127.0.0.1:5174/node_modules/.vite/deps/svelte-web3.js?v=d385d017:17704:18)

```

## To reproduce just clone and run the project with metamask installed.
