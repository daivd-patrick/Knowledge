# [React](https://reactjs.org)

## Notes

- Immediate mode simply means you specify what to redraw on every frame, there is no caching unless you specify it. And you basically redraw whenever some state changes (in a game this is going to be at frame rate).
  - In React, when some state changes, you respecify the DOM for components whose state has changed, but asynchronously the library determines how to make the DOM update more efficient on the next frame redraw.
- Retained-mode means you modify the scene graph (aka DOM) using imperative statements, it is difficult to keep your UI in synch with your models. With immediate-mode, you simply create a function f(m) over your model m to render it on each frame rate (which also often involves imperative instructions affecting the frame buffer, but the buffer can be cleared on each frame so who cares).
  - Retained-mode caches by default (often in opaque ways), which was the whole point (only re-render parts of the scene that have changed). You can roll your own caching for immediate mode, usually via some kind of invalidation scheme (use image for a node if nothing changed for this component, otherwise call that node's re-render method). On the other side, projects like React takes the retained-mode DOM and make it look more like an immediate-mode abstraction without sacrificing so much performance.
- The core premise for React is that UIs are simply a projection of data into a different form of data.
- [A React component is simply a JavaScript function that takes an object of arbitrary inputs known as props and returns React elements describing what should be rendered on the UI.](https://blog.logrocket.com/a-complete-guide-to-default-props-in-react-984ea8e6972d)

## Links

- [A practical understanding of Flux](http://sircmpwn.github.io/2015/07/20/A-practical-understanding-of-Flux.html)
- [Advanced React Component Patterns](https://egghead.io/courses/advanced-react-component-patterns)
- [Introduction to The Beginner's Guide to ReactJS](https://egghead.io/lessons/react-introduction-to-the-beginner-s-guide-to-reactjs)
- [React - Basic Theoretical Concepts](https://github.com/reactjs/react-basic#readme)
- [Didact](https://github.com/hexacta/didact) - DIY guide to build your own React.
- [ReactiFlux Learning](https://www.reactiflux.com/learning/)
- [Tom Occhino and Jordan Walke first presenting React](https://www.youtube.com/watch?v=GW0rj4sNH2w)
- [My struggle to learn react](http://bradfrost.com/blog/post/my-struggle-to-learn-react/) ([HN comments](https://news.ycombinator.com/item?id=17030865))
- [Stop writing code - Sunil Pai (2018)](https://www.youtube.com/watch?v=WYWVGQKnz5M) - Great talk.
- [The Present Future of User Interface Development](https://hackernoon.com/the-present-future-of-user-interface-development-ebd371255175)
- [React from Zero](https://github.com/kay-is/react-from-zero#readme) - Simple (99% ES2015 less) tutorial for React.
- [React is just JavaScript (2018)](https://medium.com/yld-engineering-blog/react-is-just-javascript-88600553269c)
- [React Developer Roadmap](https://github.com/adam-golab/react-developer-roadmap#readme)
- [Defining Component APIs in React](http://jxnblk.com/writing/posts/defining-component-apis-in-react/)
- [Rogue.js](https://github.com/alidcastano/rogue.js) - Nearly invisible framework for creating server-rendered React applications.
- [Diagram of modern React lifecycle methods (2018)](https://twitter.com/dan_abramov/status/981712092611989509?s=09)
- [React Fundamentals](https://github.com/ryanflorence/react-fundamentals#readme)
  - [Advanced React](https://github.com/ryanflorence/advanced-react-workshop#readme)
- [Algebraic Effects, Fibers, Coroutines . . . Oh My! - Brandon Dail (2018)](https://www.youtube.com/watch?v=cWY1QzyFhfk&feature=youtu.be)
- [Understanding React and reimplementing it from scratch Part 1: Views](https://gcanti.github.io/2014/10/29/understanding-react-and-reimplementing-it-from-scratch-part-1.html)
- [React (without the buzzwords) course](https://frontarm.com/courses/learn-raw-react)
- [Conditional Rendering with React: The Complete Guide](https://frontarm.com/articles/react-conditional-rendering/)
- [React Events Live Cheatsheet](https://frontarm.com/toolbox/react-events-cheatsheet/)
- [Complete guide to default props in React](https://blog.logrocket.com/a-complete-guide-to-default-props-in-react-984ea8e6972d)
- [A deep dive into children in React](https://mxstbr.blog/2017/02/react-children-deepdive/)
