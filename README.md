# Tableau UI
[![Tableau Supported](https://img.shields.io/badge/Support%20Level-Tableau%20Supported-53bd92.svg)](https://www.tableau.com/support-levels-it-and-developer-tools)

![Tableau UI](./assets/tableau_ui_logo.svg)

Tableau UI is a React component library containing UI components which have the look-and-feel of Tableau.

## Add Tableau UI

```npm install @tableau/tableau-ui```

## Using Tableau UI

Tableau UI requires React. If you aren't familiar with React, check out their [Getting Started](https://reactjs.org/docs/getting-started.html) document.

If you have a TypeScript project you can simply import the components and prop interfaces that you want to use, e.g.:
```ts
import * as React from 'react';
import { Button, ButtonProps } from '@tableau/tableau-ui';

const buttonProps: ButtonProps = { kind: 'outline', children: 'OK' };
const button = React.createElement(Button, buttonProps);
```

If you're using JSX, this example might look more like:
```tsx
import * as React from 'react';
import { Button } from '@tableau/tableau-ui';

const button = <Button kind='outline'>OK</Button>
```

Or, you could also choose to include the bundled javascript file in your web project just as you would any other javascript library. You will then be able to reference tableau-ui with the global `TableauUI` variable, e.g.:
```js
<script crossorigin src="https://unpkg.com/react@16/umd/react.development.js"></script>
<script crossorigin src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
<script src="tableau-ui.min.js"></script>

const button = React.createElement(TableauUI.Button, { kind: 'outline', children: 'OK' });
```

## API Documentation and Samples

Please refer to [Tableau UI Components](https://tableau.github.io/tableau-ui/) for documentation and samples.
