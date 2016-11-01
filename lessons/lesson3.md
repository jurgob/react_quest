#Lession 3
Configure your editor.

React linter is cool, but probably it is better when you have it directly in your editor.
My choise is to use Atom (https://atom.io/) and a bunch of plug in.

here's the list of plugin you should install:
 - language-babel (https://atom.io/packages/language-babel)
 - linter-eslint (https://atom.io/packages/linter-eslint)
 - js-hiperlink (https://atom.io/packages/js-hyperclick)

unluckly you need some more configuration to make linter-eslint work well, from the CRA readme:

>**A note for Atom `linter-eslint` users**

>If you are using the Atom `linter-eslint` plugin, make sure that **Use global ESLint installation** option is checked:

><img src="http://i.imgur.com/yVNNHJM.png" width="300">

Then add this block to the `package.json` file of your project:

```js
{
  // ...
  "eslintConfig": {
    "extends": "react-app"
  }
}
```

Finally, you will need to install some packages *globally*:

```sh
npm install -g eslint-config-react-app@0.3.0 eslint@3.8.1 babel-eslint@7.0.0 eslint-plugin-react@6.4.1 eslint-plugin-import@2.0.1 eslint-plugin-jsx-a11y@2.2.3 eslint-plugin-flowtype@2.21.0
```

We recognize that this is suboptimal, but it is currently required due to the way we hide the ESLint dependency. The ESLint team is already [working on a solution to this](https://github.com/eslint/eslint/issues/3458) so this may become unnecessary in a couple of months.


###a note:
facebook is deployng an editor called nuclide (https://nuclide.io/), witch is a modded version of atom. For now I still prefer Atom and the plugins I've suggested, in the feuture I will maybe change my idea 


##Video
Comming soon...
