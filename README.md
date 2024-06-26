Jaccard Index / Similarity Algorithm
====================================

For Node.js, with some modification would also run in the browser.

Usage:

```javascript
const { toBigrams, jIndex } = require('./jaccard');

const b1 = toBigrams( text1 );
const b2 = toBigrams( text2 );

const score = jIndex( b1, b2 );
// => [0, 1]
```

Where higher score is more similar.

Run `node test.js` in root for a simple test/demo.

This implementation was made to detect similarity between media filenames.

You don't have to use bigrams to generate sample set as here. You
can experiment with other ways of generating the datasets, and it
doesn't have to be text - it can be anything you can make sample set
from.


MIT License
-----------

Copyright 2020-2021 Epistemex

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
