<h1 align="center"><code> UR Experiments </code></h1>

1. [k0unty-ur-1](#k0unty-ur-1)
2. [ReaWiBu](#reawibu)
   1. [Vite Plugin](#vite-plugin)

---

# k0unty-ur-1

> Running UR experiments in different ways. Trying to use bun pnpm etc

# ReaWiBu

Installing a new project 
```sh 
bun create vite my-app
```

Run Bun server 
```sh
bunx --bun vite
```

## Vite Plugin 
- This will display errors directly on the page 

Install 
```sh 
pnpm add vite-plugin-checker -D
```

Then alter `vite.config.js`

```js 
// vite.config.js
import checker from 'vite-plugin-checker'
export default {
  plugins: [
    checker({
      // e.g. use TypeScript check
      typescript: true,
    }),
  ],
}
```