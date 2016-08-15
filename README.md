# LearningReact
MyNotesWhenLearning React

ReactDom.render(reactElement, domContainer)
The above statement will inject the react element into the container that you specify.
The 2nd arg can be any element in the entire page.

To update the properites of the element, call render againg

this.props can access all the attributes passed(it can be a value or a method itself!)

If we have multiple react components(root compoennt or single root component that gets deleted over time) in Single page app, make sure to call 
ReachDOM.unmountContainerAtNote(domContainer)


if you update a property using ReactDOM.render(). all your previous props wil be removed/updated!

Reactive State:
props are immutable:
once passed to a component, they are owned by the parent

WHEN STATE UPDATES, THE COMPONENT RE-RENDERS ITSELF!--> That is why it is called REACT! it reacts to state updates automatically!


TIP to SElf:

TIME WASTED IN SETTING UP DEV ENVIRONMENT: 3 hours- 15-Aug
If you are done wasting your time, please get back to acutal work now!




PReviously: 
In traditional DOM, inputs elements are rendered and browser manages the STATE
therefore: state of actual DOM will DIFFER FROM that of the component

IN REACT: Component will always represent the state of DOM

thus, the concept of STATE:

Event Handling:

onChange is a callBack; this is fired when the state is changed. think of it as call backTrigger in the final block of state setter.
siimilar to below:

state
{
	set{
		try{
			updateState!
		}
		finally{
			call callBack!
		}
	}
}


NOTE:
React.createClass() automatically binds the method to component instance; so no need for explicit binding!
