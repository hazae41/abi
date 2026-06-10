# ABI

ABI encoding for the web

```bash
npm install @hazae41/abi
```

[**📦 NPM**](https://www.npmjs.com/package/@hazae41/abi)

## Features

### Current features
- 100% TypeScript and ESM
- No external dependencies
- Rust-like patterns

## Usage

### Decoding

```tsx
const [string, bigint] = abi.decode([AbiString, AbiUint8], Uint8Array.fromHex(...)))
```

### Encoding

```tsx
const hex = abi.encode([AbiString, AbiUint8], ["hello world", 1n]).toHex()
```

```tsx
const hex = abi.encodePacked([AbiString, AbiUint8], ["hello world", 1n]).toHex()
```