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

let options = {
  length:50,
  ending:'...'
};

useEffect(() => {
  setText('updated');
},[]);

export const Demo = () => {
  const { text, setText } = useTruncate('initial',options);
  
  return (
    <div>
      { text }
    </div>
  );
  
};
```
