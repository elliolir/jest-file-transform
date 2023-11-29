# jest-file-transform
Custom Jest transformer turning:
* SVGs into React Components;
* The rest of file imports into filenames.

Shamelessly copy-pasted from [Create React App Scripts](https://github.com/facebook/create-react-app/blob/0a827f69ab0d2ee3871ba9b71350031d8a81b7ae/packages/react-scripts/config/jest/fileTransform.js#L4)
and updated to work with the modern version of Jest as an [ES Module](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules).

## How to Use
Just add this into your transform config
```
  transform: {
    '^(?!.*\\.(js|jsx|mjs|cjs|ts|tsx|css|json)$)': 'jest-file-transform',
  },
```