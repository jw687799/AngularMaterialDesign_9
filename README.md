# MaterialProj  
This is my learning and practice of course by using angular 9.1.4. ( Angular Material Design of Robby Millsap, Angular workflow of Victor Mejia)

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 9.1.4.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).


##Initial setup the project cmd
1) install node.js
2) install @angular/CLI
3) npm install --save @angular/material
4) npm install --save @angular/cdk
5) npm install --save @angular/animations
6) npm install --save @angular/material-moment-adapter
7) npm install --save moment
8) npm install -D prettier  ==>code formatting workflow with prettier
  .prettierrc
  .prettierignore   
9) npm instll pretty-quick npm-run-all
10) npm install jest jest-preset-angular -D  ==> this is for SNAPSHOT testing. (did not implement this one, jest.config.js)


TESTING:
1) unit testing 
1.1 cmd 'ng test' 
1.2 how to debug karma testing
'ng test' start the server -> chrome browser-> karma debug runner ( the cmd will do all these in one step)
->click on Debug button->F12->Source tab->Ctrl + P  find the file->put a breakpoint 
-> F10 step over  ->watch
                  ->call stack
-> F11 step into

2) e2e testing
2.1 'ng e2e'
running it, it complain about chrome driver version.
then do, `webdriver-manager clean`, `webdriver-manager update --versions.chrome 81.0.4044.138`, this version is my browser version,
still does not work.

2.2 have to do following to correct this issue:
npm uninstall protractor
npm install --save-dev protractor

2.3 how to put a debug point
in code, add "browser.debugger()" or "debugger". I personally like "debugger" better


