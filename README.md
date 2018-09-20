### NPM DEMO

> Before add any node package to node application, you should create package.json file by running (npm init)

1. Semantic versioning:
   In node application any package we add is added to package.json with version like ("underscore": "^1.9.1" )
   let's understood the semantic versioning system in package.json file 1.9.1 (major.minor.patch)
   whenever there is a bug in package it get fixed and increase the patch number
   whenever there is a new feature they increase minor version minor version doesn't break application
   If there is feature which can break the existing app then they increase major version

- Caret symbol(^): 1.x.x
  Caret symbol tells npm that install any available minor and patch version not the major version
- Tilde (~) 1.9.x
  Only install new patch version
- To install exact version everytime ("underscore": "1.9.1")

> Listing the install packages in an app

- To list installed package in an app we can run (npm list)
- To check only dependencies of our application not the dependencies of installed package use (npm list --depth=0)

> To view registry info for a package

- run (npm view package-name)
- to see only dependencies of package run (npm view package-name dependencies)
- to view all version that has been released of package run (npm view package-name versions)

> Installing a specific version of package

- to install exact version of pakcage (npm i mongoose@2.4.2)

> How to check outdated packages

- to check outdated packages run (npm outdated)
- to update outdated packages run (npm update)
- to check update there is a npm package called (npm-check-update) install it globally and run in any project

> To install dev dependenicies

- run (npm i package-name --save-dev)

### Global packages

- To install global package run (npm install -g package-name)
- To check oudated global package run (npm -g outdated)
- To uninstall global package run (npm uninstall -g package-name)
