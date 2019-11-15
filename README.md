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
import React, {useEffect} from 'react';
import { useTruncate } from '../src/useTruncate';

useEffect(() => {
 setText('updated');
},[]);

export const Demo = () => {
  const { text, setText } = useTruncate('initial');

  return (
    <div>
      { text }
    </div>
  );
};
```
