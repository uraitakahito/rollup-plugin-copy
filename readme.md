# rollup-plugin-copy

Original rollup-plugin-copy is [here](https://github.com/vladshcherbin/rollup-plugin-copy).

## Usage

### Configuration

#### watchTargets

Type: `boolean` | Default: `false`

Add the files specified in `targets` to the watch list

```js
copy({
  targets: [{ src: 'assets/**/*', dest: 'dist/public' }],
  watchTargets: true
})
```

## Original Author

[Cédric Meuter](https://github.com/meuter)
[Vlad Shcherbin](https://github.com/vladshcherbin)

## License

MIT
