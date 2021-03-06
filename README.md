# React app using AWS Amplify

Follow [https://aws.amazon.com/getting-started/hands-on/build-react-app-amplify-graphql](https://aws.amazon.com/getting-started/hands-on/build-react-app-amplify-graphql)

## Implement

- Create a new React application  
- Initialize GitHub repository  
- Log into AWS Management Console  
- Deploy your app with AWS Amplify  
- Automatically deploy code changes  


### Create a new React application

```
npx create-react-app amplifyapp
cd amplifyapp
npm start
```
```
PS F:\Projects\github> npx create-react-app amplifyapp
npx: installed 67 in 44.81s

Creating a new React app in F:\Projects\github\amplifyapp.

Installing packages. This might take a couple of minutes.
Installing react, react-dom, and react-scripts with cra-template...

yarn add v1.21.1
[1/4] Resolving packages...
[2/4] Fetching packages...
warning sha.js@2.4.11: Invalid bin entry for "sha.js" (in "sha.js").
info fsevents@1.2.13: The platform "win32" is incompatible with this module.
info "fsevents@1.2.13" is an optional dependency and failed compatibility check. Excluding it from installation.
info fsevents@2.3.2: The platform "win32" is incompatible with this module.
info "fsevents@2.3.2" is an optional dependency and failed compatibility check. Excluding it from installation.
[3/4] Linking dependencies...
warning "react-scripts > @typescript-eslint/eslint-plugin > tsutils@3.20.0" has unmet peer dependency "typescript@>=2.8.0 || >= 3.2.0-dev || >= 3.3.0-dev || >= 3.4.0-dev || >= 3.5.0-dev || >= 3.6.0-dev || >= 3.6.0-beta || >= 3.7.0-dev || >= 3.7.0-beta".
[4/4] Building fresh packages...
success Saved lockfile.
warning Your current version of Yarn is out of date. The latest version is "1.22.5", while you're on "1.21.1".
info To upgrade, run the following command:
$ curl --compressed -o- -L https://yarnpkg.com/install.sh | bash
success Saved 7 new dependencies.
info Direct dependencies
├─ cra-template@1.1.2
├─ react-dom@17.0.2
├─ react-scripts@4.0.3
└─ react@17.0.2
info All dependencies
├─ cra-template@1.1.2
├─ immer@8.0.1
├─ react-dev-utils@11.0.4
├─ react-dom@17.0.2
├─ react-scripts@4.0.3
├─ react@17.0.2
└─ scheduler@0.20.2
Done in 298.00s.

Initialized a git repository.

Installing template dependencies using yarnpkg...
yarn add v1.21.1
[1/4] Resolving packages...
[2/4] Fetching packages...
info fsevents@2.3.2: The platform "win32" is incompatible with this module.
info "fsevents@2.3.2" is an optional dependency and failed compatibility check. Excluding it from installation.
info fsevents@1.2.13: The platform "win32" is incompatible with this module.
info "fsevents@1.2.13" is an optional dependency and failed compatibility check. Excluding it from installation.
[3/4] Linking dependencies...
warning "react-scripts > @typescript-eslint/eslint-plugin > tsutils@3.20.0" has unmet peer dependency "typescript@>=2.8.0 || >= 3.2.0-dev || >= 3.3.0-dev || >= 3.4.0-dev || >= 3.5.0-dev || >= 3.6.0-dev || >= 3.6.0-beta || >= 3.7.0-dev || >= 3.7.0-beta".
warning " > @testing-library/user-event@12.8.3" has unmet peer dependency "@testing-library/dom@>=7.21.4".
[4/4] Building fresh packages...
success Saved lockfile.
success Saved 16 new dependencies.
info Direct dependencies
├─ @testing-library/jest-dom@5.14.1
├─ @testing-library/react@11.2.7
├─ @testing-library/user-event@12.8.3
├─ react-dom@17.0.2
├─ react@17.0.2
└─ web-vitals@1.1.2
info All dependencies
├─ @testing-library/dom@7.31.2
├─ @testing-library/jest-dom@5.14.1
├─ @testing-library/react@11.2.7
├─ @testing-library/user-event@12.8.3
├─ @types/aria-query@4.2.2
├─ @types/jest@26.0.24
├─ @types/testing-library__jest-dom@5.14.0
├─ css.escape@1.5.1
├─ css@3.0.0
├─ lz-string@1.4.4
├─ min-indent@1.0.1
├─ react-dom@17.0.2
├─ react@17.0.2
├─ redent@3.0.0
├─ strip-indent@3.0.0
└─ web-vitals@1.1.2
Done in 63.06s.
Removing template package using yarnpkg...

yarn remove v1.21.1
[1/2] Removing module cra-template...
[2/2] Regenerating lockfile and installing missing dependencies...
info fsevents@2.3.2: The platform "win32" is incompatible with this module.
info "fsevents@2.3.2" is an optional dependency and failed compatibility check. Excluding it from installation.
info fsevents@1.2.13: The platform "win32" is incompatible with this module.
info "fsevents@1.2.13" is an optional dependency and failed compatibility check. Excluding it from installation.
warning " > @testing-library/user-event@12.8.3" has unmet peer dependency "@testing-library/dom@>=7.21.4".
warning "react-scripts > @typescript-eslint/eslint-plugin > tsutils@3.20.0" has unmet peer dependency "typescript@>=2.8.0 || >= 3.2.0-dev || >= 3.3.0-dev || >= 3.4.0-dev || >= 3.5.0-dev || >= 3.6.0-dev || >= 3.6.0-beta || >= 3.7.0-dev || >= 3.7.0-beta".
success Uninstalled packages.
Done in 68.64s.

Created git commit.

Success! Created amplifyapp at F:\Projects\github\amplifyapp
Inside that directory, you can run several commands:

  yarn start
    Starts the development server.

  yarn build
    Bundles the app into static files for production.

  yarn test
    Starts the test runner.

  yarn eject
    Removes this tool and copies build dependencies, configuration files
    and scripts into the app directory. If you do this, you can’t go back!

We suggest that you begin by typing:

  cd amplifyapp
  yarn start

Happy hacking!
PS F:\Projects\github> cd .\amplifyapp\
PS F:\Projects\github\amplifyapp> npm start

> amplifyapp@0.1.0 start F:\Projects\github\amplifyapp
> react-scripts start

```