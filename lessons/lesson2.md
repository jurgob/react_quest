#Lesson Two:
Familiarize with create-react-app command

create-react-app comes with some fancy thing ready for use, the linter and the test.
It have also a way to build your app easily.

##Linter
to see the linter in action start the app with:

```
npm start
```

Then try to change something in "a wrong" way.

Like go to App.js and add ```var test``` before the App class declaration:

```
  var test;
  class App extends Component {
```

now both the terminal and the browser console should display the error: ```4:5  warning  'test' is defined but never used  no-unused-vars```

delete ```var test```  and the error will disappear

##test

to start the test run:

```
npm test
```

it will start an interactive test mask. If you change any file , the chanin will re-run.
try to change ```<h2>Welcome to React</h2>``` to ```<h2Welcome to React</h2>```. it will broke the test, if you fix it, the tool chane will became green again.

##test (not interractive modeand coverage)

if you want to run the tests in non interactive mode you have to set CI env variable to true.
run ```CI=true npm test``` to run them in a non - interactive way.

to know the test coverage you can run ```npm test -- -coverage```


## build
to build your app, you can use the run command. to build your app and test it against a web service do:
```
npm run build
cd build
python -m SimpleHTTPServer 8000
```
you can use this python command or any other static web server command you want.


## Video:
Coming soon...
