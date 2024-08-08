
# React
Everything I have learnt so far in React!

## useState
useState is a React Hook that allows you to create a state variable.

### Import using
`import { useState } from "react";`

### Initializing
Initialize the state at the top of the function.  
`const [count, setCount] = useState("")`  

The first value, `count` represents the name of the state.  
The second value, `setCount` represents the name of the function that updates the state.  
The third value, `""` inside the round brackets sets the initial state. In this case, the initial state is set to an empty string.

### Updating State
Call function to update state. In this case, we have named the function `setCount`.  
We cannot directly change the state by saying `count = 12`. This is mutating the state and state variables are immutable.  
Instead, we use the update function that we determined earlier.

`setCount(count + 1)`

### Updating Objects or Arrays
JavaScript spread operator can help us update just one property while keeping the rest the same.  
```
const [userInfo, setUserInfo] = useState({
    name: "John",
    occupation: "Dog trainer"
    height: "170cm"
})
```
```
const updateOcc = () => {
    setUserInfo(currentInfo => {
        return {...currentInfo, occupation: "Driver"}
    })
}
```

The spread operator tells JavaScript to return the object as is, and what follows is the property that is going to be updated, with its new value.




