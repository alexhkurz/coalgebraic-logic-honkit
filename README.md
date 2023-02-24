# README 

How I tried to make this book:

## Basic setup

### Step 1

Get a local server up and running.

https://honkit.netlify.app/setup.html

```
npm install honkit --save-dev
npx honkit init
npx honkit serve
```

### Step 2

Make honkit work with latex.

add `book.json`:

```
{
    "plugins": ["mathjax"]
}
```

build with

```
npx honkit build
```

yields error

```
(base) ~/alexhkurz-at-github/coalgebraic-logic-honkit > npx honkit build  
info: 6 plugins are installed 
info: 6 explicitly listed 
info: plugin "highlight" is loaded
info: plugin "search" is loaded
info: plugin "lunr" is loaded
info: plugin "fontsettings" is loaded
info: plugin "theme-default" is loaded
Error [PluginError]: Error with plugin "mathjax": Unexpected token '<<'
    at createError (/Users/alexanderkurz/node_modules/error/typed.js:31:22)
    at new createError (/Users/alexanderkurz/node_modules/error/wrapped.js:88:19)
    at /Users/alexanderkurz/node_modules/honkit/lib/plugins/loadPlugin.js:67:23
    at _fulfilled (/Users/alexanderkurz/node_modules/q/q.js:854:54)
    at /Users/alexanderkurz/node_modules/q/q.js:883:30
    at Promise.promise.promiseDispatch (/Users/alexanderkurz/node_modules/q/q.js:816:13)
    at /Users/alexanderkurz/node_modules/q/q.js:877:14
    at runSingle (/Users/alexanderkurz/node_modules/q/q.js:137:13)
    at flush (/Users/alexanderkurz/node_modules/q/q.js:125:13)
    at processTicksAndRejections (internal/process/task_queues.js:79:11) {
  type: 'plugin',
  plugin: 'mathjax',
  causeMessage: "Unexpected token '<<'",
  origMessage: "Unexpected token '<<'",
  fullType: 'plugin~!~error.wrapped-unknown'
}
```

### Step 3

(planned)

Copy some content into a folder `content`.

Adjust the file `SUMMARY.md` accordingly.





