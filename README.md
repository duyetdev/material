Material Design for AngularJS Apps
=======

[Material Design](http://www.google.com/design/spec/material-design/) is a specification for a unified system of visual, motion, and interaction design that adapts across different devices.

Our goal is to deliver a lean, lightweight set of AngularJS-native UI elements that implement the material design system for use in Angular SPAs. 

This project is still in early preview. It is a complementary effort to the [Polymer](http://www.polymer-project.org/) project's [paper elements collection](http://www.polymer-project.org/docs/elements/paper-elements.html).

## Demo Site

You can see these components in action at http://material.angularjs.org

## Development

This project is in early development via a small core team of [Ionic Framework](http://ionicframework.com/) and [AngularJS](http://angularjs.org) developers. We don't have guidelines yet for broader community involvement, although we hope to have some soon.

For issues, including progress on accessibility support for these UI elements, see the [Issue Tracker](https://github.com/angular/material/issues)

See [CONTRIBUTING.md](https://github.com/angular/material/tree/master/CONTRIBUTING.md) for information
on structure, documentation, and code conventions.

## Usage

In its current early state, use AngularJS Material Design at your own risk.  APIs are changing rapidly.

When [v0.0.1 is released](https://github.com/angular/material/issues?milestone=2&state=open), the project will be more usable.  But everything is subject to rapid change until beta is ready.

Nevertheless, if you wish to use AngularJS Material Design, here are the steps (note that what the dependencies are and how to use them will change soon):

1. `npm install`
1. `bower install`
1. `gulp build`
1. Include `jquery.js`
1. Include `angular.js`
1. Include `angular-animate.js`
1. Include `config/lib/angular-animate-sequence/angular-animate-sequence.js`
1. Include `config/lib/angular-animate-sequence/angular-animate-stylers.js`
1. Include `dist/material-design.js`
1. Include `dist/material-design.css`

### File Structure

- Components belong in `src/components/{componentName}`
- Component modules must be named `material.components.{componentName}`
- Templates for directives are declared inline
- Gulp builds files to `dist` folder, which is not version controlled (read below)

### Commit Conventions

- http://github.com/ajoslin/conventional-changelog
- git commit-msg hook available [here](https://github.com/angular/angular.js/blob/master/validate-commit-msg.js).  Place it in `.git/hooks/commit-msg`, and run `chmod +x .git/hooks/commit-msg`. It will validate your commit messages for you.

### Development 

- `npm install` for gulp deps
- `git submodule update --init` to add icons subfolder
- `bower install` for angular deps
- `gulp build` (alias `gulp`) to build, add `--release` flag to uglify & strip console.log.
- `gulp watch` to build & rebuild on changes
- `gulp validate` to test and jshint
- `gulp jshint` to run jshint
- `gulp karma` to test once
- `gulp karma-watch` to test & watch for changes
- `gulp docs` to build docs into dist/docs

### Documentation

- See `docs/README.md`.
