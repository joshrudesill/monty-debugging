# Bug Report!

## Describe

**What is happening? What do you see?**
The database schema wasnt setup properly

**What _should_ be happening? What do you want to see?**
The name column should be type VARCHAR(20) not INT

## Isolate

**Is this problem client side? Server side? Elsewhere? How do you know?**
Database. While I was setting up my database I ran the table setup query then the insert query which I had already fixed (the value orders were not correct) and it said name was the incorrect type

**What line of code is the error happening on?**
database.sql LINE 4

Paste the relevant code here:

```js
"name" VARCHAR(20) NOT NULL,
```

And describe what it's doing wrong:
It is accepting a number rather than a string

**What tools did you use to isolate the error?**

- [ ] `console.log()`
- [ ] Chrome debugger (_Sources_ panel)
- [ ] VSCode debugger
- [ ] Chrome Network Panel
- [ ] Postman
- [x] Postico

<!-- Briefly describe how the tool helped you, and how you used it -->

There was an error when trying to run the setup queries

## Fix

❗ Don't try to fix before first **describing** and **isolating!**

Briefly describe your fix:
Changed the type from INT to VARCHAR(20) of the name column

**What tools did you use?**

- [ ] Fix one line of code. Then test using the debugger or `console.log()`s.
- [ ] Google search
- [ ] Ask a pod mate for help
- [x] Escalate

**Results**

<!-- Go back to your original description. Is the app behaving how you want it to, now? Describe the bug, technically: what was your code doing wrong, and how did you fix it. -->
