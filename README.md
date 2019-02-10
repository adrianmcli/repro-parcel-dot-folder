# A bug in 

When the entry file is inside a dot folder, I get the following error in my browser:

```
Uncaught SyntaxError: Unexpected token <
```

It seems like the server might be serving the HTML as JS for some reason (instead of serving the real JS file).

## To test

1. Clone the repo
2. Run `npm run without-dot`, and observe that everything works fine in the browser.
3. Run `npm run with-dot`, and observe that the error occurs in the browser.
