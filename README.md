# vue-ssr-hmr-thead-issue

Copied from `vite/packages/playground/ssr-vue` and added table with thead to src/App.vue.

```bash
% yarn
% yarn dev
```

Most updates to children of the `thead` element cause HMR issues, try this patch for example:

```bash
diff --git a/src/App.vue b/src/App.vue
index 1c652b7..28f7bec 100644
--- a/src/App.vue
+++ b/src/App.vue
@@ -4,7 +4,7 @@
       <thead>
         <tr>
           <th>Hello</th>
-          <th>Update this textContent, for example, and trigger HMR</th>
+          <th>Update this textContent, for example, and trigger HMR!!</th>
         </tr>
       </thead>
     </table>
```

![Screenshot of console error](https://i.imgur.com/2V8vnp0.png)
