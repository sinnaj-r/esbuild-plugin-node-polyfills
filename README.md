# ESBuild Plugin Node Polyfills

Provides NodeJS Polyfills similar to Webpack's "node" option

## Usage

1. Install Package (`npm install -D esbuild-plugin-node-polyfills` or `yarn add --dev esbuild-plugin-node-polyfills`)
2. Install the required mocks from the peer-dependencies
3. Use in your ESBuild Script:

```js
import { ESBuildNodePolyfillsPlugin } from "esbuild-plugin-node-polyfills";

// Your ESBuild Config
const config = {
  plugins: [ESBuildNodePolyfillsPlugin],
};
```

## Modules with Polyfills

- `buffer`
- `crypto`
- `http`
- `https`
- `os`
- `path`
- `stream`
- `zlib`
- `url`
- `events`
- `process`
- `util`
- `_stream_duplex`
- `_stream_passthrough`
- `_stream_readable`
- `_stream_transform`
- `_stream_writable`

## Modules which will be resolved to `false`

- `tls`
- `assert`
- `fs`
- `net`
