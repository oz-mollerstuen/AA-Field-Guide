# 2/17/23

* 8:35 - Working on Proposal/research 
* 9:15 - Finish proposal, begin research
* 10:30 - Continued API research
* 11:15 - Researching other AA and health tracker sites for ideas on forms
* 12:00 - WIP:Lunch: Reponded to email, more research and adding links
* 01:24 - Responded to emails about API
* 01:51 - Added readme with a baisic description
* 02:33 - More research, testing in test app
* 03:20 - More research, Begin building bare bones of app.
* 04:00 - Watching [videos](https://www.youtube.com/watch?v=ngfYZ0U-emg) on best ways to build app
* 04:30 - Add CapstoneApp-experiments to github, more research
* 04:50 - End Of Day: More research and Helpful websites added

#
# 02/24/24

* 8:00 - Begin research on REACT version of project
* 8:30 - Update Proposal and start research
* 9:27 - Built bones of react project
* 9:50 - Add header and footer to project
* 10:20 - Add some style to see header and footer
* 10:50 - Researched additional libraries for react
* 11:45 - Narrowing down which style of calendar I want in app, work on 'Journal' 
* 1:10 - Testing calendar in app
* 1:35 - Implementing Sass
* 2:20 - install web-pack and update files
* 2:50 - finish webpack install and added sass to webpack file.
* 3:05 - vs code for app completely frozen. Taking a break
* 3:25 - Back at it, did not chuck computer out the window
* 4:15 - Restarted computer, react is slowing and freezing in vs code. & bug squashing
* 4:59 - WIP end of day *phew* Will continue to debug webpack

#
# 3/3/23

* 8:00 - Re-init cap-research, start research on notepad feature
* 8:40 - Found new templates to research and take styling notes
* 9:00 - Imported too many libraries. New project, simplicity in mind
* 9:45 - [Researching Google stater kit](https://github.com/google/web-starter-kit)
* 10:20 - [Different approach](https://medium.com/@sanderdebr/building-a-workout-tracker-with-react-and-firebase-part-1-e1b13c073135)
* 11:00 - Fixing bugs in App.jsx
* 11:45 - Installing MUI libraries and building sign-in screen
* 12:20 - WIP - taking lunch, continue working on sign-in
* 12:55 - Back from lunch, will continue sign-in
* 1:35 - finishing up sign-in/up/out, set up Firebase
* 2:05 - Integrating Firebase, adding components
* 2:36 - Customizing calendar, adding dashboard and tracker components
* 3:21 - Add activity tracker, snackBar
* 4:00 - Finish activity tracker, begin de-bugging
* 4:45 - Fighting with material-ui issues, slowly fixing them
* 6:15 - Back from 30 minute rest
* 7:00 - WIP: Calling it a day

#
#  3/04/23

* 11:00 - Begin day, work on bugs in code
* 12:27 - Material-UI is not fully compatible with react-dom v. 6, finding a work around
* 1:00 - trying to refactor to use chakra ui
* 2:00 - Still refactoring
* 3:30 - adding additional packages, listing in research.md
* 5:00 - setting up "ColorModeSwitcher"
* 5:45 - Re-building sideBar
* 7:20 - going through all material-ui components, researching replacements for chakra-ui integration using [chakra-ui docs](https://chakra-ui.com/)
* 9:00 - WIP: Calling it a day, continue with last three errors tomorrow

#
# 3/7/23

* 8:00 - begin day, error hunting
* 9:00 - Still fixing bugs: 

* config_theme_signinup__WEBPACK_IMPORTED_MODULE_3__.default is not a function


#### 9:50 - Cannot find fix to webpack error. Possible work arounds:
* Restart project
* further research
* uninstall webpack, reinstall

#

* 10:00 - Uninstall (global) and reinstall (global) did not work 
![errors - signin](https://user-images.githubusercontent.com/115112679/223510016-2579dc51-c9ab-491d-b65f-3a4c4e0a7607.png)

* 11:00 - uninstalling all packages and reinstalling them. This includes webpack, chakra-ui, and emaotion. deleting node modules and lock.json

* 12:00 - scrapping project and starting over. Again.

* 12:50 - attempt to use some of my code to rebuild app

* 1:50 - fixed bundle.js issue by importing and adding PasswordForget to routes. Working on why nothing shows on page.

* 2:30 - Routes give an error of

```
No routes matched location "/" 
```
* 3:00 - Still figuring out routes.
* 3:58 - New errors and warnings!
```
bundle.js:95019 Warning: Received `true` for a non-boolean attribute `item`.

If you want to write it to the DOM, pass a string instead: item="true" or item={value.toString()}.
```

And

```
bundle.js:95019 Warning: Received `false` for a non-boolean attribute `xs`.

If you want to write it to the DOM, pass a string instead: xs="false" or xs={value.toString()}.

If you used to conditionally omit it with xs={condition && value}, pass xs={condition ? value : undefined} instead.
```
AND

```
You are loading @emotion/react when it is already loaded. Running multiple instances may cause problems. This can happen if multiple versions are used, or if multiple builds of the same version are used.
```

because WHY NOT?

#
* 4:46 - New errors that I currently trying to fix:
```
bundle.js:1857 Uncaught ReferenceError: Cannot access 'config' before initialization
```

#
# Wednesday 3/8/23

### 2:45 - I forgot to log everything today up until now:
* fixed syntax errors in firebase.js and reconfigured app so firebase will actually create and store information for sign-up and sign-in
* Calendar displayed until auth was updated, working on that now.
* cannot read properties of undefined (reading 'auth') - Firebase was initialized incorrectly
* Uncaught FirebaseError: "projectId" not provided in firebase.initializeApp. - I kept the "PROJECT_NAME". Fun times!
* ERROR 'firebase' is not defined, 'firebaseConfig' is not defined  no-undef. WHERE??
* Uncaught FirebaseError: Firebase: Error (auth/invalid-api-key).
* export 'default' (imported as 'firebase') was not found in 'firebase/app'

#
* 3:15 - Working on FirebaseError: Firebase: Error (auth/invalid-api-key).

* 3:50 - Career services, still working on api-key issue.