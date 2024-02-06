# Bug Report!

## Describe

The npm start script was pointing to a file that didnt exist
**What is happening? What do you see?**
When I went to setup my npm start script to include --watch I noticed it wasnt pointing to the usual server/server.js

**What _should_ be happening? What do you want to see?**
It should be pointing to our entry point file. In this case server/server.js

## Isolate

**Is this problem client side? Server side? Elsewhere? How do you know?**
Server Side

**What line of code is the error happening on?**
Package.json - 8

Paste the relevant code here:

```js
  "start": "node --watch server/server.js"
```

And describe what it's doing wrong:
It is pointing to a file which doesnt exist, therefore npm wont be able to run anything when npm start is ran

**What tools did you use to isolate the error?**

- [ ] `console.log()`
- [ ] Chrome debugger (_Sources_ panel)
- [ ] VSCode debugger
- [ ] Chrome Network Panel
- [ ] Postman
- [ ] Postico
- [x] Noticed when setting up workspace

<!-- Briefly describe how the tool helped you, and how you used it -->

VSCode

## Fix

❗ Don't try to fix before first **describing** and **isolating!**

Briefly describe your fix:
Changed the npm start script to point to server/server.js which is the entry point

**What tools did you use?**

- [x] Fix one line of code. Then test using the debugger or `console.log()`s.
- [ ] Google search
- [ ] Ask a pod mate for help
- [ ] Escalate

**Results**

<!-- Go back to your original description. Is the app behaving how you want it to, now? Describe the bug, technically: what was your code doing wrong, and how did you fix it. -->
