# vue-ssr-hmr-thead-issue

Copied from vite/packages/playground/ssr-vue and added table with thead to src/App.vue.

```
% yarn
% yarn dev
```

Most updates to children to the `thead` element cause HMR issues (eg. adding `!` to innerText).

![Screenshot of console error](https://imgur.com/2V8vnp0)
