## Hints

### See things more clearly

Try removing the `-m-2` style from the tree so you can see what's happening more clearly. Don't forget to checkout dev tools either!

### Define your base case and recursive case

Recursion always requires two things:

1. The recursive case — this is where the magic happens
2. The base case — the is where the magic _stops_, otherwise you recurse infinitely until your computer blows up or you accidentally open up a wormhole to another dimension

To do this you need a switch of some kind (maybe a `v-if`?), and a value that changes with each step in the recursion.

### Where do you place the recursion?

You can either place the recusion before or after (or both) what the component is rendering. Each will give you opposite results:

```html
<!-- Before -->
<template>
  <div>
    <ChristmasTree />
    Render this
  </div>
</template>
```

```html
<!-- After -->
<template>
  <div>
    Render this
    <ChristmasTree />
  </div>
</template>
```

The wrong one will give you an upside-down tree.

### Slots

You _will_ need to use named slots here. It's a crucial part of the puzzle.
