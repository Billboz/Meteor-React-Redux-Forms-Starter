# Meteor React, Redux-Forms, and optimal set up.

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

Clone the repo and and have fun.

If you would like to build this yourself then for my own practice and maybe your benefit I am going to put the steps I took below.

FYI - I am on a Mac, I use Atom https://atom.io/ and iTerm2 https://www.iterm2.com/.  So some of this might need to be adjusted to your setup. I am learning and this setup should not be contrued as optimal or tested.  Actually, if you can help me with this I would greatly appreciate it :)
Good Luck, Have Fun!

Steps:

1. Create your Meteor project
2. Delete and create the file and folder structure that [Meteor recommends](https://guide.meteor.com/structure.html#example-app-structure).  I don't set up the testing because I haven't learned about testing yet, that will come later.
3. Because I have so much to learn I enjoy all the help I can get so I set up the [Meteor flavored ESLint](https://guide.meteor.com/code-style.html#eslint-installing) packages.  There are a couple steps to do but the result is AWESOME!
4. Run this in terminal ```meteor npm install --save-dev babel-eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-meteor eslint-plugin-react eslint-plugin-jsx-a11y eslint-import-resolver-meteor eslint```
5. As the page instructs you place the scripts in the 'package.json' file and finish the instructions.
6. 
