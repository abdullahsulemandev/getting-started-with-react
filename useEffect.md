

We studied usestate useEffect hook in Reactwh ich is used to handle side effects.
 state managment
 syntax ---->  [state, 			stateSetter]
 		|			|
 		correct state		{stateSet}
 		
 we can handle this in three ways:
 1. No array
 2. Empty array
 3. Dependency array
 
 
 1. No Array: The effect runs after every render.
 useEffect(() => {}); // Instagram following example

2. Empty array:	The effect runs only once, after the initial render.
useEffect(() => {
}, []);				// Infinite loop

				useEffect(() => {
					setState()
				})
				

3. Dependency array:   The effect runs only when the specified dependencies change.
useEffect(() => {
}, [Value1]);
	|
	The dependency array in useEffect minimizes unnecessary
	re-runs by ensuring the effect only runs when specified 
	dependencies change.