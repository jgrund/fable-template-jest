# Fable Jest Template

This template can be used to generate a simple testing app with
[Fable](http://fable.io/) and [Jest](https://facebook.github.io/jest/).

You can find more templates by searching `Fable.Template` packages in
[Nuget](https://www.nuget.org).

## Requirements

* [dotnet SDK](https://www.microsoft.com/net/download/core) 2.0 or higher
* [node.js](https://nodejs.org) 6.11 or higher

> npm comes bundled with node.js, but we recommend to use at least npm 5. If you
> have npm installed, you can upgrade it by running `npm install -g npm`.

Although is not a Fable requirement, on macOS and Linux you'll need
[Mono](http://www.mono-project.com/) for other F# tooling like Paket or editor
support.

## Installing the template

In a terminal, run `dotnet new -i Fable.Template.Jest` to install or update the
template to the latest version.

## Creating a new project with the template

In a terminal, run `dotnet new jest` to create a project in the current
directory. Type `dotnet new jest -n MyApp` instead to create a subfolder named
`MyApp` and put the new project there.

> The project will have the name of the directory. You may get some issues if
> the directory name contains some special characters like hyphens

## Building and running the app

* Install JS dependencies: `npm i`
* Install F# dependencies: `dotnet restore`
* Run the tests `dotnet fable npm-run test`
* Run the tests and output code coverage `dotnet fable npm-run coverage`
* Run the tests in watch mode:
  * In one terminal `dotnet fable start`
  * In a second terminal `npm run test-watch`
    * This will allow you to run all, or just a subset of tests, and will
      re-test the changed files on save.
