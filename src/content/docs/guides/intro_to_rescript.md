---
title: Intro to ReScript
description: A guide to getting started with ReScript.
---

[ReScript](https://rescript-lang.org/) is a modern language with strong types with a JavaScript like syntax that compiles to human readable JavaScript. It has a super fast compiler that provides instant feedback. It's somewhat similar to TypeScript, but the two languages have different goals.

__TypeScript__ is a superset of JavaScript, which means all valid JavaScript is valid TypeScript. TypeScript doesn't force you to be strict with your types and has plenty of escape hatches like the `any` type or being able to turn off type checking with `@ts-ignore`. It's a layer of types on an untyped language. It's an improvement over JavaScript, but it's still not a sound type system. Sound types mean that we can guarantee that the types are correct, which you can't do if you have an `any` type or are able to type cast to the wrong type. 

```ts
const value: any = { foo: "bar" }

console.log(value.bad.key) // no type errors, but this is a runtime error!
```

__ReScript__ is a completely different language from JavaScript with it has a JS like syntax that fits right into the JS ecosystem. It's easy for JavaScript developers to pick up and you'll probably be productive with it on your first day with the language. You can think of it as just the "good parts" of JS with strong types baked in. Oh, and you don't need to clutter your code with type annotations since the compiler is smart enough to get the types correct for you.

```ts
let value = { "foo": "bar" } // you can't use an any type
Console.log(value["bad"]["key"]) // This expression has type {"foo": string}It has no field bad
```

## The main features of ReScript
You can check out the [ReScript docs](https://rescript-lang.org/docs/manual/latest/introduction) if you want to dive into the language, but here's a quick overview of how the language works.

### Creating things is easy
You don't have to worry about when to use `function`, `var`, `const`, or `let`. ReScript just has one way to make a value or function and thats by using `let`.
```tsx
let name = "Josh"

let greet = (name) => `Hello ${name}`
```

### You don't need to annotate types

### Values are immutable by default

### Everything is an expression

### The pipe operator

### Pattern matching

### Variant types
