# Node + Express + Express Templates ARE BUSTED!

## Task

* Find all the errors in the code and fix them so the app runs
* There are _multiple_ errors (~15 of them). The app won't run intil they're _all_ fixed.
* As you make it through one error, be on the lookout for the next one.
* __ALL__ files are in play (except `package-lock.json`).

## Getting started

* First, run `npm i` to install all the dependencies
* Then run `npm run dev` to start the app.
* Start fixing!

### Notes

* LOOK AT SPELLING ERRORS AND/OR TYPOS!
* Variable names are CASE SENSITIVE!
* **SERIOUSLY** almost _every_ file is in play!
* In these files I used the shorter `req` and `res` in place of `request` and `response`. They're the same objects, just using shorter variable names.
* Don't forget the HTML files!! Make sure things like links work!

## Resolved Issues

1. `package.json` > misspelled `nodemon` in `dev` script
2. `package.json` > missing `nodemon` dependency
3. `app.js` > http module not imported
4. `app.js` > PORT and HOSTNAME don't match usage
5. `routes/rangers.js` > missing parenthesis for `find` method
6. `routes/rangers.js` > `rangersModel` import path incorrect
7. `routes/rangers.js` > `router` is not exported
8. `model/db.js` > missing comma between array items
9.  `model/db.js` > `modules` should be `module`
10. `app.js` > rootController is not used
11. `routes/index.js` > template should be `res.render('template'...`
12. `views/partials/home.html` > link contains no href
13. `views/partials/ranger-list.html` > map function param should be `ranger`
14. `views/partials/ranger-detail.html` > variable should be `ranger`
15. `.gitignore` > missing `node_modules` exclude