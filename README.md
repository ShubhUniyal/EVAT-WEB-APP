# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
HEAD
# EVAT-Web-Application
EVAT is a mobile application designed to streamline vehicle management. This repository contains the DevOps codebase for the EVAT web application.
=======

# EVAT Mobile Application

## Table of Contents

- Introduction
- Features
- Installation
- Usage
- Development
- Contributing
- Code Quality
- Git Etiquette
- License
- Contact

## Introduction

The EVAT mobile application allows users to find the nearest vehicle charging station efficiently and is designed to streamline vehicle management. This repository contains the DevOps codebase for the EVAT web application.

## Features

- User Registration
- User Login
- Add Vehicle
- View Vehicle Details

## Installation

To get started with the project, follow these steps:

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/EVAT-web-application.git
    ```

2. Navigate to the project directory:

    ```bash
    cd EVAT-web-application
    ```

3. Install dependencies:

    ```bash
    npm install
    ```

## Usage

To start the development server, run:

```bash
npm start
```

## Development

To run the front end project locally, from the root project run:

```bash
cd front_end_project && npm run start
```

To run the back end project locally, from the root project run:

```bash
cd back_end_project && npm run start
```

To launch both the node server and react app, run:

```bash
npm run devall
```

Note: npm run devall isn’t working currently.
To launch the node server alone, run:

```bash
npm run server
```

This can be used by API developers to test their API through POSTMAN.
Development should follow the Feature branch git workflow. Important: Never commit directly to main.
When pulling the latest from GitHub, you may need to run npm install  if any packages were added or removed in past commits. If you are experiencing errors unrelated to the code you are writing (or before writing any), try running npm install.

## Contributing

We welcome contributions! Please follow these steps to contribute:
**Fork the repository.**
**Create a new branch:**

```bash
git checkout -b feature/your-feature
```

Commit your changes:

```bash
git commit -m 'Add some feature'
```

Push to the branch:

```bash
git push origin feature/your-feature
```

## Code Quality

### Linting

Code quality is enforced by ESLint, which is configured as a custom eslint plugin shared across the entire project in `eslintrc.js`. Each package/app requires its own `.eslintrc.js` file.

- Components, component directories, component files, and stories all use PascalCase / UpperCamelCase.
- Variables and functions use camelCase.
- Single quotes for strings.
- Do not use string interpolation for CSS classes.
- Do not use CSS-in-JS, StyledComponents, or Emotion CSS.

## Git Etiquette

### Branching

Branches are used for isolated feature development and should always branch from the source they intend to merge into. This means that a branch created from `main` must always end up in `main`.

```bash
Using the example branches of main -> feature-1 -> feature-2…
❌ Do not merge feature-1 into main before feature-2 is merged.
❌ Do not merge feature-2 directly into main, only its parent branch.
✅ Do branch feature-2 from main since it should not depend on feature-1.
Note: If it’s entirely necessary to merge feature-1 before feature-2, ensure that no manual commits are made in feature-2 between the last commit & merge commit to main of feature-1.
```

## Commit Messages

There are no hard constraints imposed on commit messaging. Instead, the following guidelines show a best-practice approach to producing consumable commit messaging.
The preferred format for a commit message looks like this. Note that only the body is required:

```bash
# format...
"type?(scope?): body..."

# examples...
"fixed some issue"
"fix: fixed some issue"
"fix(US-123): fixed some issue"
"fix(component): fixed some issue"
```

## Commit Types

- **type** refers to what kind of commit is being made. Some example values are:
  - `--build` // related to build processes
  - `--chore` // small cleanup activities or other pedantry
  - `--ci` // related to continuous integration activities
  - `--docs` // documentation work
  - `--feat` // feature work
  - `--fix` // bugfixes or hotfixes
  - `--perf` // performance tuning & optimization
  - `--refactor` // code refactoring
  - `--revert` // reverting previously committed changes
  - `--style` // styling changes
  - `--test` // changes to tests

- **scope** provides context to the commit type, most commonly a MS planner ticket or some project name.
- **body** refers to the bulk of the commit message, which can break up into header and footer sections delimited by newlines.
  - A **header** is the body section on the first line of the commit message.
  - A **footer** is entered a full newline separated from the header and may contain any length of UTF-8 content.

## APIs

Here are the APIs that will be used in the EVAT Mobile application:

### User Management

- User Registration API
- User Login API
- User Profile API

### Vehicle Management

- Add Vehicle API
- View Vehicle Details API
- Update Vehicle API
- Delete Vehicle API

### Charging Station

- Find Nearest Charging Station API
- Real-time Charging Station Availability API

### Maps Integration

- Google Maps API (for displaying maps and locations)
- Geolocation API (for getting the user’s current location)

### Backend

- MongoDB API (for database operations)

### License

For the license, the MIT License is a popular choice for open-source projects.
MIT License

Copyright (c) 2024 Chameleon-company

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
 768657f (Readme.md)
