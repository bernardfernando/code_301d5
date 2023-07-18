Readings: State and Props

Below you will find some reading material, code samples, and some additional resources that support the topic for this class and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

Reading
[React lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

## Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

Render
componentDidMount - this happens immediately after mounting.

## What is the very first thing to happen in the lifecycle of React?

### Mounting

_When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount,_ and UNSAFE*componentWillMount all occur in this order during mounting.*
_Put the following things in the order that they happen:_ componentDidMount, render, constructor, componentWillUnmount, React Updates\_

## What does componentDidMount do?

## componentDidMount()

_This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount()._

Videos

# React State Vs Props

## What types of things can you pass in the props?

Props allow data from one component to be passed on to another as an argument.

## What is the big difference between props and state?

_State holds information. Props can be accessed by the child component. State cannot be accessed by child component/_

## When do we re-render our application?

_When React needs to update the app with some new data.. usually this happens as a result of a user interacting with the app or some external data coming through via an asynchronous request or some subscription model._

## What are some examples of things that we could store in state?

_Any kind of JS value, including objects._

## Bookmark and Review

[React Docs - State and Lifecycle](https://legacy.reactjs.org/docs/state-and-lifecycle.html)
[React Docs - handling events](https://legacy.reactjs.org/docs/handling-events.html)
[React Tutorial through ‘Developer Tools’](https://react.dev/learn/tutorial-tic-tac-toe)
[React Bootstrap Documentation](https://react-bootstrap.github.io/)
[Boootstrap Cheatsheet](https://getbootstrap.com/docs/5.0/examples/cheatsheet/)
[Bootstrap Shuffle - a class “sandbox”](https://bootstrapshuffle.com/classes)
[Netlify](https://www.netlify.com/)
