
# lesson 1:
create a react app.


npm install -g create-react-app
create-react-app mandi-mont


npm start

open App.js

change "hello world" with "mandi mont"



# lesson 2
check our app


npm run lint

add some wrong Tab
npm run lint

npm run test

broke your app

npm run test


# lesson 3
configure Atom
install atom
https://facebook.github.io/react/blog/2016/07/22/create-apps-with-no-configuration.html

those ones are the plugins I use (you can always check nuclide)

language-babel
js-hiperlink
linter-eslint

unluckly, you need to configure eslint globally:


# lesson 4
let's build our first widget.

## part a) the beginning
Components are basically 'custom HTML tag'.
But in react you use the 'HTML' inside your js file. this is called 'JSX'
let's say you can see your Component as a function witch accept attributes (props) and return HTML (jsx )
(props) => JSX
let's do one:

const Mandify = () => (
  <div>
    Mandi
  </div>
)

import Mandi from './Mandi'

<Mandi />

## part b) add some props
const Mandify = ({name}) => (
  <div>
    Mandi, {name}
  </div>
)

<Mandi name="vigji" />



# lesson 5
let's add storybook. TDD-ish develop with react

## part a) install storybook
https://github.com/kadirahq/react-storybook

npm i -g getstorybook
cd my-react-app
getstorybook


npm run storybook


## part b) the Mandify's story:

create :
stories/Mandi.js

storyof()

## part c) snapshot tests for a storyof
npm run snapshot test//TODO
change your package.json, the test

# lesson 6
React statements, if , for and others


# lesson 7
components with lifecicles
now that you are becommig a react expert, I can tell you that  sometimes your components can be something more then a function like (props) => HTML :)
They can have a state, and they can use the lifecicles components.

https://facebook.github.io/react/docs/react-component.html

## part a) the state
let's do a Counter

## part b) the lifecicles method
initialize the counter


#lession 8
user interaction

controlled vs not controlled:

## part a) uncontrolled form

## part b) controlled

you will probably want to use on of the already existings tools


#lession 9
fetch some data


#lesson 10
React PropTypes, aka be safe

React team said it's temporary, check out Flow or Typescript if you want to "see the future"

#lesson 11
React Router
