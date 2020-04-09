## `<Formik />`
`<Formik>` is a component that helps you with building forms. It uses a render props pattern made popular by libraries like React Motion and React Router.

### Installation
You can install Formik with NPM, Yarn, or a good ol' <script> via unpkg.com.

NPM

`npm install formik --save  `

or

`yarn add formik`


### The Gist 


Formik keeps track of your form's state and then exposes it plus a few reusable methods and event handlers (handleChange, handleBlur, and handleSubmit) to your form via props. handleChange and handleBlur work exactly as expected--they use a name or id attribute to figure out which field to update.


Example:

https://imgur.com/a/T11cHop



## Custom Hooks

A custom Hook is a JavaScript function whose name starts with ”use” and that may call other Hooks. For example, useFriendStatus below is our first custom Hook:


```import { useState, useEffect } from "react";

function useFriendStatus(friendID) {
  const [isOnline, setIsOnline] = useState(null);

  useEffect(() => {
    function handleStatusChange(status) {
      setIsOnline(status.isOnline);
    }

    ChatAPI.subscribeToFriendStatus(friendID, handleStatusChange);
    return () => {
      ChatAPI.unsubscribeFromFriendStatus(friendID, handleStatusChange);
    };
  });

  return isOnline;
}

```


we can use it like that:


```
function FriendStatus(props) {
  const isOnline = useFriendStatus(props.friend.id);

  if (isOnline === null) {
    return "Loading...";
  }
  return isOnline ? "Online" : "Offline";
}
```


### Rules of Hooks

* Only Call Hooks at the Top Level

* Only Call Hooks from React Functions

(instead you can
✅ Call Hooks from React function components.
✅ Call Hooks from custom Hooks
)

