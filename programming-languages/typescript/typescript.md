# [TypeScript](https://github.com/Microsoft/TypeScript)
[TS Handbook](https://www.typescriptlang.org/docs/handbook/basic-types.html) and [this article](https://toddmotto.com/typescript-introduction) are great intros.

## Notes
- TypeScript can figure the return type out by looking at the return statements, so we can also optionally leave this off in many cases
- You really shouldn’t use arrow function as class members. Arrow functions are duplicated in memory for each class instance, while proper method members are written once in your class’s prototype and shared between all instances.
- [Unlike classes, an interface is a virtual structure that only exists within the context of TypeScript. The TypeScript compiler uses interfaces solely for type-checking purposes.](https://toddmotto.com/classes-vs-interfaces-in-typescript)

## Links
- [React & Redux in TypeScript - Static Typing Guide](https://github.com/piotrwitek/react-redux-typescript-guide#readme)
- [Opening Remarks by Anders Hejlsberg (2018)](https://www.youtube.com/watch?v=wpgKd-rwnMw)
- [Ultimate React Component Patterns with Typescript 2.8](https://levelup.gitconnected.com/ultimate-react-component-patterns-with-typescript-2-8-82990c516935)
- [Very opinionated front end boilerplate](https://ts-react-boilerplate.js.org/)
- [Babel 7 + TypeScript](http://artsy.github.io/blog/2017/11/27/Babel-7-and-TypeScript/)
- [Classes vs interfaces in TS](https://toddmotto.com/classes-vs-interfaces-in-typescript)