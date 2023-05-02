# Setting up Jest for basic automated testing.

Setup steps with links and bash commands for the Jest testing framework:

### Install Node.js and npm: 

Jest is built on top of Node.js, so you'll need to install Node.js and its package manager, npm, if you haven't already. You can download the latest version of Node.js from the official website: https://nodejs.org/en/download/

### Create a new project:

Create a new directory for your project and navigate to it in your terminal:

```
mkdir my-project
cd my-project
```

### Initialize a new npm project:

Run the following command to create a new package.json file for your project, which will allow you to manage your project's dependencies and scripts:

```
npm init -y
```

- The -y flag will accept all default settings for the package.json file.

### Install Jest: 

Run the following command to install Jest as a development dependency for your project:

```
npm install --save-dev jest
```

This will install the latest version of Jest and add it to your package.json file as a dev dependency.

### Create a test file:

Create a new file called sum.test.js in your project's root directory, and add the following code:

```js
function sum(a, b) {
  return a + b;
}

test('adds 1 + 2 to equal 3', () => {
  expect(sum(1, 2)).toBe(3);
});
```

This code defines a simple sum function and a single test case that verifies that the function correctly adds 1 and 2 to equal 3.

### Run your tests:

Run the following command to run your tests using Jest:

```
npx jest
```

This will execute your test cases and report any failures or errors.

That's it! With these steps, you should be able to set up and run automated unit tests for your JavaScript code using Jest. You can find more information on Jest's documentation site: https://jestjs.io/docs/en/getting-started.