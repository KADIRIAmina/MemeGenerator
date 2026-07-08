what react can't handle:
- side effects: interacting with outside system ( localStorage; react isn't automatically updating the changes, API/Databases, subscription; React doesn't know how to connect to outside system ) 

- how to deal with this ? we use useEffect
- it's a function that we're calling frpm react like useState
- how to use it ? inside the call back function inside useEffect we put the code that's
- but this's not enough, we need also the optional dependencies array
- cuz we'll be still runnig the function inside useEffect after each render, and the function itself is rundering the page and so.

- dependencies array is an array of values that react is going to watch between one render and the  next, it helps us to run the code inside useEffect only if this values changes (between one renbder and the next)

- not using it will cause the run of that code after each render, what may cause an infinit loop 
- it's called dependencies array cause the call bzack function inside useEffect depends on it

- when we want to run the code inside the useEffect only one time we use an empty array

- cleanup functions

- useRef; refs are similar to state, except changing a ref doesn't cause a re render (we use it to access the dom nodes without assigning ids to elements)
