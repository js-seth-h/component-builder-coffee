# fork, Why?

[builder-coffee-script](https://github.com/component/builder-coffee) is not working on my dld server without supporting SSE4.

this is a version adopting [crc32](https://github.com/beatgammit/crc32).

# builder-coffee-script

Coffee Script plugin for [component-builder2](https://github.com/component/builder2.js).

- Caches compilations
- Sourcemap support

## Example

```js
var build = require('component-builder2');
var coffee = require('component-builder-coffee');

build.scripts(nodes)
  .use('scripts', build.plugins.js())
  .use('scripts', coffee())
  .use('coffeescripts', coffee());

build.pipe(process.stdout);
```

You could put your coffee-script files in `.scripts` or create your own field like `.coffeescripts`.

## License

The MIT License (MIT)

Copyright (c) 2014 junsik &lt;js@seth.h@google.com&gt;

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.