# rollup jsx plugin

This is a simple wrapper around [jsx-transform](https://github.com/alexmingoia/jsx-transform). Make sure to go check that out for options.

# depracated

I originally made this project for buble, before JSX support went in. have a look at [/buble-react-rollup-starter](https://github.com/yamafaktory/buble-react-rollup-starter) for a great example of usage without this plugin.

Install it with `npm install rollup-plugin-jsx`

Use it like this in your config:

```js
import jsx from 'rollup-plugin-jsx'

export default {
  dest: 'build/app.js',
  entry: 'src/index.js',
  plugins: [
    jsx( {factory: 'React.createElement'} )
  ],
  sourceMap: true
}

```

For a more complete example, see [buble-react-rollup-starter](https://github.com/yamafaktory/buble-react-rollup-starter)
