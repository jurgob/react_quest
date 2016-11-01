#Lesson 4
let's build our first widget.

## part a) the beginning
Components are basically 'custom HTML tag'.
But in react you use the 'HTML' inside your js file. this is called 'JSX'
let's say you can see your Component as a function witch accept attributes (props) and return HTML (jsx )
(props) => JSX
let's do one:

create in ```src``` the file ```Mandify.js``` with this content:

```js
import React from 'react'

const Mandify = () => (
  <div>
    Mandi
  </div>
)

export default Mandify
```

you can find the file here: https://github.com/jurgob/mandi-mond/blob/481980e959b8ad12573801e34a152b9a0b260380/src/Mandify.js

now you can use it inside App.s adding those line

```js
import Mandi from './Mandi'

  ...
  <p className="App-intro">
    To get started, edit <code>src/App.js</code> and save to reload.
  </p>
  <Mandify />
```
the file is here:
https://github.com/jurgob/mandi-mond/blob/481980e959b8ad12573801e34a152b9a0b260380/src/App.js


You will see a "Mandi" text displayed in your page

## part b) add some props

let's learn how to pass props to our component. Just change Mandify.js and App.js as following:


###Mandify.js
```js
const Mandify = ({name}) => (
  <div>
    Mandi, {name}
  </div>
)
```

###App.js
<Mandi name="jimmy" />


you should see now "Mandi, jimmy"

here you can see the changes:
https://github.com/jurgob/mandi-mond/commit/5302e1c3af1eddf751357870da1eaf05f282f909

##Video
Comming soon...
