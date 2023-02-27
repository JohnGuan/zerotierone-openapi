# ZeroTierOne OpenAPI

Complete version of ZeroTierOne's OpenAPI

> ⚠️ This is not an official document by ZeroTier Inc.
>
> 🤩 This is the full version with additions based on the official documentation and source code, especially the controller API.

## API Client

### typescript-axios

> zerotierone-api-ts-axios

[
    ![NPM Version](https://img.shields.io/npm/v/zerotierone-api-ts-axios?style=flat-square)
    ![NPM Downloads](https://img.shields.io/npm/dw/zerotierone-api-ts-axios?style=flat-square)
](https://www.npmjs.com/package/zerotierone-api-ts-axios)

#### Install

```shell
npm i zerotierone-api-ts-axios
```

```shell
yarn add zerotierone-api-ts-axios
```

#### Usage

```typescript
import {
  Configuration,
  StatusApi,
  NetworkApi,
  ControllerApi,
  PeerApi,
} from "zerotierone-api-ts-axios";

// create configuration
const configuration = new Configuration({
  basePath: "/path/to/your/backend",
});

// export configured api instances
export const statusApi = new StatusApi(configuration);
export const networkApi = new NetworkApi(configuration);
export const controllerApi = new ControllerApi(configuration);
export const peerApi = new PeerApi(configuration);

// export models and other exports
export * from "zerotierone-api-ts-axios";
```
