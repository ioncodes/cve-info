# vscode-typescript-mocha

<h1 align="center">Minimal visual studio code, typescript and mocha project boiler plate</h1>

<p align="center">  
  <b>A simple project to bootstrap a typescript project with multiple the settings files preconfigured.</b></br>
 
  <sub>Made with ❤️ by <a href="https://github.com/paganaye">Pascal Ganaye</a></sub>
</p>

<br />

## ❯ Why

It is not rocket science but it is a bit fiddly to get this three component rights.

### Features

- **TypeScript compilation** done in memory, we don't save any javascript files anywhere.
- **Test Runner** Mocha tests are available instantly, a couple samples tests are provided.
- **Visual Studio Code Debugging** is configured and works instantly.

### Caveat

This project only applies for Node projects. 
There is no browser and no web server in this project.

## ❯ Table of Contents

- [Getting Started](#-getting-started)
- [Recommended plugins](#-recommended-plugins)
- [VSCode integration](#-vscode-integration)
- [License](#-license)


## ❯ Getting Started

### Step 1: Set up the Development Environment

You need to set up your development environment before you can do anything.

Install [Node.js and NPM](https://nodejs.org/en/download/)


### Step 2: Copy the Project

```bash
git clone https://github.com/paganaye/vscode-typescript-mocha.git <NameOfYourProject>
```
or download a ZIP. 

Then install the dependencies.

```bash
cd <NameOfYourProject>
npm install
```

### Step 3: Run VSCODE

```bash
code .
```

> This starts visual studio code in the current folder.

Press <kbd>control</kbd>+<kbd>shift</kbd>+<kbd>B</kbd>

You should see

```
> mocha

  test1
    √ The dog should bark

  #test2
    √ The cat should meow


  2 passing (8ms)
```
## ❯ Recommended plugins

We recommend you to install the extension below.  

https://marketplace.visualstudio.com/items?itemName=hbenl.vscode-mocha-test-adapter


![mocha test explorer plugin](documentation/mocha-test-explorer.png)

This plugin wil make your tests appear in the Test Explorer and let you run individual test files or tests directly from the source.

![test explorer](documentation/running-from-test-explorer.png)


## ❯ VSCode integration

The editor intellisense works from the get go.
The tests can be run and debugged directly from the source file.

![intellisense in the source editor](documentation/typescript-intellisense.png)


### ❯ Debugger in VS Code

There is no need to build the app.
Just set a breakpoint and hit <kbd>F5</kbd> in your Visual Studio Code.


![debugging a test](documentation/debugging-a-test.png)

We have two launch command preconfigured for you:

The first: `Debug current Test file` is for Mocha test 

The second: `Debug current Typescript file` is specifically for debugging files that are not specifically tests. 

### ❯ Configured files

We have configured the files below, any of them can be tweaked further to accomodate your needs.


    package.json
    tsconfig.json
    .gitignore
    .mocharc.json
    .vscode/settings.json
    .vscode/tasks.json
    .vscode/launch.json

## ❯ Customization

While you're accustomed with environment you can delete all the files in `src`, `test`, `documentation` and replace them with yours.

## ❯ Improvement

If you want to contribute to this repository please fork it and submit a pull request if you want to.

## ❯ License

[MIT](/LICENSE)


