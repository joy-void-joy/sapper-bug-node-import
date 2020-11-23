Bug report repo for Sapper
===

This is a repo for [issue]

This repo is taken directly from "sveltejs/sapper-template#rollup", the only file modifications are those under routes/. Other files have been deleted to help read the project easily, but have no impacts on the bug.

This bug also apply if using webpack.  
See the issue above to learn more

How to reproduce
---
If you run ``npm run dev`` and head over to ``localhost:3000/redirect`` you will see the list of the current files  
However if you go to ``localhost:3000`` and click on ``redirect`` you will see ``Failed to resolve module specifier 'fs'`` instead  
In both cases, the console note that
```
'fs' is imported by src/routes/redirect.svelte, but could not be resolved – treating it as an external dependency
```
