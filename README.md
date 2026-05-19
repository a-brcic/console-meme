# console.meme() 🎭

> "At an Angular conference in Belgrade, a speaker mentioned that `console.log` 
> supports CSS styling. Most people just nodded. We went home and built `console.meme()`."

## What is this?

A fun discovery turned into something nobody asked for, but everyone deserves.

`console.meme()` extends the native `console` object to render memes directly 
in the browser's developer console — because why not.

## Usage

```js
console.meme()        // Guess I Will Die Meme
console.meme(1)       // Perfect Meme
console.meme(1, 2)    // Disappointed Cricket Fan Meme (any 2+ arguments)
```

Open your browser console and try it. You're welcome.

## The tech behind it

Turns out `console.log` supports CSS styling via the `%c` directive:

```js
console.log('%c ', 'background-image: url(...); padding: 75px;');
```

This is wrapped in an IIFE to avoid polluting the global scope 
(other than `console.meme`, obviously).

## Origin story

Spotted at an Angular conference in Belgrade. One speaker casually mentioned 
CSS support in `console.log`. Most developers in the room had never heard of it.
A few of us went home, and `console.meme()` was born.

## Stack
- Vanilla JavaScript
- CSS-in-console witchcraft
- Questionable life choices
