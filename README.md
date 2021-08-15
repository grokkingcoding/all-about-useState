![Image for short guide](https://source.unsplash.com/PkbZahEG2Ng)

# About

- This is a guide about using the React hook called useState:

# All about useState

1. To hold data in a component we utilise useState in React. It is a hook for managing state in a component.

** An important note: useState does not persist state between browser refresh. For that, you would still need to use localstorage. **

2. This is how you would import the useState hook in a React component.

```

import React, { useState } from 'react';

```

3. This is how we would import the useState hook and use it in a React component.

```

export default function Component() {

    const [someObj, setObj] = useState({});

...

```

4. So in this component, someObj holds the state of the component. When you call setObj(newData) with some new data, useState will overwrite the data in "someObj" and replace it with new data.

5. For exmaple, if you wanted to set the state when the component first renders, then you could use setObj in the useEffect hook like this:

- the console log will show the updated state of someObj

```

useEffect(() => {
        setObj(newData);
}, []);

console.log('log someObj')
console.log(someObj)

```
