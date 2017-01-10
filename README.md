# angular2-folder-structure-example
File and Folder Structure Example for an Angular 2 App with Redux

This repo is a mock representation of the file and folder structure of a large scale Angular 2 application with redux. The architecture is meant to follow the [Angular Style Guide](https://angular.io/docs/ts/latest/guide/style-guide.html). The files are stubs only and not meant to create an actual functioning application. Files contain comments of what they are expected to contain. `README.md` files have been included in folders where further explaination is required.

## Mock Application Concept

The application that this is modelling is an adoption tracking app between families and cats. There is standard CRUD operations for both families and cats, as well as an authentication flow.

## General File / Folder Comments

### Barrel Files (`index.ts`)
For simpler ES6 Module import paths, it is reccomended to add barrel files (`index.ts`) to each folder in the tree that re-exports the contents of the containing files and folders. This allows for shorter import paths as well as easier refactoring if you need to move files/folders around.

> When using services across modules, there have been issues with import statements that go through more than one folder level. For instance: `core/authentication/authentication.service.ts` must be imported using `../core/authentication` instead of `../core`. 