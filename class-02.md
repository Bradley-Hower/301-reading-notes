# React State and Props

## React lifecycle

Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

In the React lifecycle, there four major stages:

1.0 **contructor** - Called before being mounted. 
  Can:
  - Assign state using `this.state`.
  - Bind event handle methods to instance.
  - Hold `super(props)` if component is a subclass.

2.0 **render** - Runs update.

3.1 **componentDidMount** - DOM and refs updated prior. Run any network request, initialize the DOM, or set up any subscriptions. Remember to unsubscribe componentWillUnmount(). Rare use case, `setState()`, due to rerender.

3.2 **Unmounting - componentWillUnmount** - Unmounting is called afterwards when a component is removed from the DOM.

*Rarely, **static getDerivedStateFromProps()** is another stage that occurs between the contructor and render. This method is used when the state depends on updates in the props. Runs update.*

*Additional, **componentDidUpdate()**. A method used to perform network requests upon changes.


![Lifecycle Diagram](filler)


