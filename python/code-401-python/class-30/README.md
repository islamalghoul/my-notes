[MainPage](../../../README.md)
# Building Your Own Hooks
Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class.

Building your own Hooks lets you extract component logic into reusable functions.

When we were learning about using the Effect Hook, we saw this component from a chat application that displays a message indicating whether a friend is online or offline
Now let’s say that our chat application also has a contact list, and we want to render names of online users with a green color. We could copy and paste similar logic above into our FriendListItem component but it wouldn’t be ideal
Instead, we’d like to share this logic between FriendStatus and FriendListItem.

Traditionally in React, we’ve had two popular ways to share stateful logic between components: render props and higher-order components. We will now look at how Hooks solve many of the same problems without forcing you to add more components to the tree.

xtracting a Custom Hook
When we want to share logic between two JavaScript functions, we extract it to a third function. Both components and Hooks are functions, so this works for them too!

A custom Hook is a JavaScript function whose name starts with ”use” and that may call other Hooks.
There’s nothing new inside of it — the logic is copied from the components above. Just like in a component, make sure to only call other Hooks unconditionally at the top level of your custom Hook.

Unlike a React component, a custom Hook doesn’t need to have a specific signature. We can decide what it takes as arguments, and what, if anything, it should return. In other words, it’s just like a normal function. Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it.
Using a Custom Hook
In the beginning, our stated goal was to remove the duplicated logic from the FriendStatus and FriendListItem components. Both of them want to know whether a friend is online. 