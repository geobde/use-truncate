## Usage

Import the hook:

```javascript
import { useTruncate } from 'use-truncate';
```

### Truncate text

```javascript
const { text, setText } = useTruncate(string);
```

### Full example

```javascript
import React from 'react';
import { useTruncate } from '../src/useTruncate';

export const Demo = () => {
  const { text, setText } = useTruncate('hello world');

  return (
    <div>
      {text}
    </div>
  );
};
```

## Specification

### `usePosition()` input

- `settings: object` - [options]
  - `settings.length` - truncating text  by the number of words,
  - `settings.ending` - add string i.e (...) ti the end of the word`),
