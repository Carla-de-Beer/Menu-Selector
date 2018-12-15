# Menu Selector

[![Build Status](https://circleci.com/gh/Carla-de-Beer/Menu-Selector.png?&style=shield&circle-token=:circle-token)](https://circleci.com/gh/Carla-de-Beer/Matrix-Library)
[![GitHub issues](https://img.shields.io/github/issues/Carla-de-Beer/Menu-Selector.svg?style=flat-square)](https://github.com/Carla-de-Beer/Menu-Selector/issues)

A simple menu selector, written in plain vanilla JavaScript (ES6), that allows a user to book a meal, consisting of two courses, for two diners respectively. The project can be run simply with a local server.

### Booking rules

- Each person must have at least two courses, one of which must be a main.
- Each diner cannot have more than one of the same course.
- There is only one piece of cheesecake left.
- Pierre, the snobby waiter, will not let you have prawn cocktail and salmon fillet in the same meal.
- The total bill amount is displayed when at least one dish has been selected.
- An error message is displayed when I try to select an invalid menu combination.

### Technical notes

- The folowing npm packages were used:
  - ESList: `npm install --save-dev eslint`.
  - Jest: `npm install --save-dev jest`.
- ESLint is applied and configured inside the `.eslintrc.js` file. Linting can be run with the command `npm run lint`.
- Unit tests for the utility helper methods are written in Jest and can be run with the command `npm run test`.
- Continous integration is incorporated into the respository by means of CircleCI.
- SCSS is used as the CSS library (at present a FileWatcher is set up via the IDE to handle the mapping to CSS; ideally this should form part of a Webpack bundling process).
- jQueryUI is used for the dialog messages. A more contemporary UI library could be considered for future development work.

### Currently outstanding

- [ ] Module bundling with Webpack 4 to be added (this has been implemented separately, but could not be successfully combined with Jest in time for the submission).

### Future development

- The menu data is provided by means of mockdata in a locally stored JSON file. In reality the data will be received live from a backend server. In this case the three course `<div>`'s in the UI need to be converted to scrollable elements.
