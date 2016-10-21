# Meteor React, Redux-Forms, and 'my' optimal set up.

Feature list:

 * Meteor 1.4.1.2
 * Recommended folder/file structure
 * Meteor specific ESLint and family :)
 * Bootstrap 4
 * React
 * Redux
 * Redux-Forms and a slew of dependencies
 * React-Router
 * Maybe Redux-Saga
 * Accounts-UI

This set up is a great start, with the best javascript framework for developer experience, and some of the most proven and supported cutting edge packages for a scalable and performant app.  I think it is a great way to prepare for what Apollo Stack will bring to Meteor in version 1.5.

Clone the repo and hack away.

If you would rather build it yourself I will leave the steps I took below for your use.

FYI - I am using a Mac and for a text editor I use Atom https://atom.io/.  So some of the following might need to be adjusted to your setup.  

If you have expertise with Meteor and/or these packages then please offer any help you think can benefit this project. :)

Good Luck, Have Fun!

Steps:

1. Create your Meteor project ```meteor create your_project```
2. Delete and create the file and folder structure that [Meteor recommends](https://guide.meteor.com/structure.html#example-app-structure).  I don't set up the testing because I haven't learned about testing yet, that will come later.
3. Because I have so much to learn, I enjoy using all the help I can get, so I set up the [Meteor flavored ESLint](https://guide.meteor.com/code-style.html#eslint-installing) packages.  Sublime and Webstorm directions are on this page as well.  There are a couple steps to do but the result is AWESOME!
4. Run this in terminal ```meteor npm install --save-dev babel-eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-meteor eslint-plugin-react eslint-plugin-jsx-a11y eslint-import-resolver-meteor eslint``` If you get some errors because some dependencies are no longer available. There is a bash command on the [AirBnB ESLint github](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb) that you can run  ```(
  export PKG=eslint-config-airbnb;
  npm info "$PKG@latest" peerDependencies --json | command sed 's/[\{\},]//g ; s/: /@/g' | xargs npm install --save-dev "$PKG@latest"
)```
5. Now copy the scripts and put them into your ```package.json``` file.
6. In your Meteor folder create a ```.eslintrc``` file and type the following into it ```{ "extends": "airbnb" }```
7. Be sure you have the supporting packages in your text editor.  For atom, you will need to install:

```
apm install language-babel
apm install linter
apm install linter-eslint
```

8. Now go type some jibberish into a .js file to see if you get a bunch of errors.  Cool huh!
9. Enter the following commands in terminal:
10. ```npm install bootstrap@4.0.0-alpha.5``` &nbsp;&nbsp;&nbsp;&nbsp;[LINK TO SOURCE](https://v4-alpha.getbootstrap.com/getting-started/download/)
11. ```meteor npm install --save react react-dom``` &nbsp;&nbsp;&nbsp;&nbsp;[LINK TO SOURCE](https://guide.meteor.com/react.html#using-with-meteor)
12. ```meteor npm install --save react-router``` &nbsp;&nbsp;&nbsp;&nbsp;[LINK TO SOURCE](https://guide.meteor.com/react.html#using-react-router)
13. ```meteor add react-meteor-data``` &nbsp;&nbsp;&nbsp;&nbsp;[LINK TO SOURCE](https://atmospherejs.com/meteor/react-meteor-data)
14. ```npm install --save redux-form``` &nbsp;&nbsp;&nbsp;&nbsp;[LINK TO SOURCE](https://github.com/erikras/redux-form)

Time for a break since two dependencies didn't get installed.
```
├── UNMET PEER DEPENDENCY react-redux@^4.3.0 || ^5.0.0-beta
├── UNMET PEER DEPENDENCY redux@^3.0.0
```
So I tried to ```npm install --save react-redux@^4.3.0 || ^5.0.0-beta``` and the other one and both failed.  After reading what people have done with similar problems I just ran ```npm install --save redux``` and ```npm install --save redux-form``` and ```npm install --save react-redux``` again and this time they all installed without issue!!
15. 
