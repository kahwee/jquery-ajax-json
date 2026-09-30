# jquery-ajax-json

Post a JSON body through jQuery's Ajax API. The module also registers
`$.postJSON` on the jQuery instance it loads.

## Install and use

```sh
npm install jquery-ajax-json jquery
```

In a browser bundle with jQuery available:

```js
const postJSON = require('jquery-ajax-json')
postJSON('/api/items', { name: 'demo' }, data => console.log(data))
```

The function returns jQuery's Ajax result, uses POST with
`Content-Type: application/json`, and serializes the supplied data.

## Development

`npm run build` runs ESLint, Browserify, and UglifyJS. `npm test` is a failing
placeholder. This checkout retains its historical build dependencies; current
Node compatibility has not been established.
