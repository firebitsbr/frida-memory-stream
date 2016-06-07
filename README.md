# frida-memory-stream

Create a stream from one or more memory regions.

## Example

```js
const memoryStream = require('@viaforensics/frida-memory-stream');

const m = Process.enumerateModulesSync()[0];
memoryStream(m.base, m.size).pipe(networkStream);
```
