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

yields an error discussed in this [issue](https://github.com/honkit/honkit/issues/325). Following the instructions there seems to solve the problem:

```
npm install --save-dev gitbook-plugin-mathjax@1
npm install mathjax@2.7.6 --save-dev
```

### Step 3

Copy some content into a folder `content`.

Adjust the file `SUMMARY.md` accordingly.





