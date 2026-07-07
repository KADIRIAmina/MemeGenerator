- state allows us to save information from one render to another
- conditional rendering alllows us to render a content accoding to some condition (as it's name shows) 
- in functional programing, a pure fonction gives us the same output for the same input 
- immutability, as shown when we don't change props, and states (only doing it by using setState)

- avoiding side effects; 
- every time we change local state react re-render the component to render the most recent version of it, this causes unfinit loop
- to avoid this "side effects", we use a hook useEffect 