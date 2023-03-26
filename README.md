This repo is designed to accompany the related egghead.io video course:
[https://egghead.io/courses/publish-javascript-packages-on-npm](https://egghead.io/courses/publish-javascript-packages-on-npm)

---

# Example

```sh
$ npm install sensitive-words --save
```

```javascript
const {sensitiveWords} = require('sensitive-words')
// ES2015 modules
import {sensitiveWords} from 'sensitive-words'

const filtered = 
  sensitiveWords(
    'The new apple macbook pro will have a touchbar',
    ['pro', 'touchbar']
  )

console.log(filtered)
// The new apple macbook *** will have a ***
```