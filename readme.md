# rollup-plugin-copy

Original `rollup-plugin-copy` is [here](https://github.com/vladshcherbin/rollup-plugin-copy).

## Usage

### Additional Configuration

#### watchTargets

Type: `boolean` | Default: `false`

Add the files specified in `targets` to the watch list

```js
import copy from "@uraitakahito/rollup-plugin-copy";

export default {
  input: "src/main.js",
  output: {
    file: "dist/bundle.js",
    format: "es",
  },
  plugins: [
    copy({
      targets: [
        { src: "src/index.html", dest: "dist" },
        { src: "src/image/**/*", dest: "dist/image" },
      ],
      verbose: true,
      watchTargets: true,
    }),
  ],
};
```

And run:

```console
% rollup --config --watch
```

A sample repository can be found [here](https://github.com/uraitakahito/hello-my-rollup-plugin-copy).

## Original Author

- [Cédric Meuter](https://github.com/meuter)
- [Vlad Shcherbin](https://github.com/vladshcherbin)

## License

MIT
