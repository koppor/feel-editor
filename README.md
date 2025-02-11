# @bpmn-io/feel-editor

Embeddable Editor for FEEL expressions.

## Usage

To get started, create a feel-editor instance:

```JavaScript
import FeelEditor from '@bpmn-io/feel-editor';

const editor = new FeelEditor({
  container
});
```

Optionally, you can provide a starting document and listen for changes:

```JavaScript
const editor = new FeelEditor({
  container,
  onChange,
  onKeyDown,
  onLint,
  value
});
```

### Variables

You can provide a variables array that will be used for auto completion. The Variables
need to be in the following format:

```JavaScript
const editor = new FeelEditor({
  container,
  variables: [
    {
      name: 'variablename to match',
      detail: 'optional inline info',
      info: 'optional pop-out info'
    }
  ]
});
```

## Hacking the Project

To get the development setup make sure to have [NodeJS](https://nodejs.org/en/download/) installed.
As soon as you are set up, clone the project and execute

```
npm install
npm start
```

## License

MIT
