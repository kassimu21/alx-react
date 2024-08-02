We would like to add a way to log to the console every time a component has been mounted and every time it is about to unmount.

To not repeat the same code everywhere, create a HOC component in task_4/dashboard/src/HOC/WithLogging.js:

The component should log to the console Component NAME_OF_THE_WRAPPED_COMPONENT is mounted on componentDidMount()
The component should log to the console Component NAME_OF_THE_WRAPPED_COMPONENT is going to unmount on componentWillUnmount()
Modify the displayName of the HOC to always display WithLogging(NAME_OF_THE_WRAPPED_COMPONENT) in the React Chrome Extension or for debugging
NAME_OF_THE_WRAPPED_COMPONENT should be the name of the wrapped component or class. If the wrapped element has no name it should default to Component
