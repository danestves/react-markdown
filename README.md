# react-markdown

React component to parse and render Flavored Markdown content

This component made use of [@danestves/markdown](https://github.com/danestves/markdown) to render a content using markdown in a React application.

## Usage

Install it with:

```bash
npm i -S @danestves/react-markdown

yarn add @danestves/react-markdown
```

Import it with:

```js
import React from 'react';
import Markdown from '@danestves/react-markdown';

function App() {
  return (
    <Markdown
      tagName='div'
      content='**Hello World in Bold!**'
      parser={
        {
          // @danestves/markdown options
        }
      }
    />
  );
}
```

- You cand send any native DOM attribute to the Markdown component.
- The default `tagName` is a `div`.
- The value of `parser` is an empty object by default.
- The `content` is required.

## Run test

You have 4 ways to run tests.

- `npm t`: run the test once
- `npm run test:fix`: run the test and fix the snapshots
- `npm run test:watch`: run the test and keep watching changes
- `npm run test:report`: run test and generate a coverage report
