# rollup-plugin-copy

Original `rollup-plugin-copy` is [here](https://github.com/vladshcherbin/rollup-plugin-copy).

## Usage

### Additional Configuration

#### watchTargets

Type: `boolean` | Default: `false`

Add the files specified in `targets` to the watch list

```js
import copy from '@uraitakahito/rollup-plugin-copy';
import { defineConfig } from 'rollup';
const config = defineConfig(
  [
    {
      input: 'src/main.js',
      output: [
        {
          dir: 'dist',
          format: 'es',
          preserveModules: true,
        },
      ],
      plugins: [
        copy({
          targets: [
            { src: 'src/index.html', dest: 'dist' },
          ],
          verbose: true,
          watchTargets: true,
        }),
      ],
    },
  ]
);
export default config;
```

And run:

```console
% rollup --config --watch
```

## Original Author

- [Cédric Meuter](https://github.com/meuter)
- [Vlad Shcherbin](https://github.com/vladshcherbin)

## License

MIT
