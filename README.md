# ext-storage-sync

[![npm version](https://img.shields.io/npm/v/ext-storage-sync)](https://npmjs.com/package/ext-storage-sync)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue.svg)](https://www.typescriptlang.org/)
[![CI Status](https://github.com/theluckystrike/ext-storage-sync/actions/workflows/ci.yml/badge.svg)](https://github.com/theluckystrike/ext-storage-sync/actions)
[![Discord](https://img.shields.io/badge/Discord-Zovo-blueviolet.svg?logo=discord)](https://discord.gg/zovo)
[![Website](https://img.shields.io/badge/Website-zovo.one-blue)](https://zovo.one)
[![GitHub Stars](https://img.shields.io/github/stars/theluckystrike/ext-storage-sync?style=social)](https://github.com/theluckystrike/ext-storage-sync)

> Chrome Extension utility library for modern extension development with sync storage support.

Part of the [Zovo](https://zovo.one) family of privacy-first Chrome extensions and developer tools.

## Overview

`ext-storage-sync` is a TypeScript utility library that provides enhanced storage synchronization capabilities for Chrome extensions. Built with modern Chrome Extension development best practices.

## Features

- ✅ **TypeScript Support** - Fully typed for better developer experience
- ✅ **Promise-based API** - Modern async/await syntax
- ✅ **MV3 Compatible** - Works with Manifest V3 extensions
- ✅ **Lightweight** - Minimal dependencies
- ✅ **Privacy-First** - No data collection, all local

## Installation

### From npm

```bash
npm install ext-storage-sync
```

### From Source

```bash
# Clone the repository
git clone https://github.com/theluckystrike/ext-storage-sync.git
cd ext-storage-sync

# Install dependencies
npm install

# Build the project
npm run build
```

## Usage

### Basic Usage

```typescript
import { Library } from 'ext-storage-sync';

// Initialize the library
const lib = new Library();
lib.init();

// Your code here
```

### Using with Chrome Extension

```typescript
import { Library } from 'ext-storage-sync';

// In your extension's background script or popup
const storage = new Library();
storage.init();

// Access chrome.storage.sync
chrome.storage.sync.get(['key'], (result) => {
  console.log(result.key);
});
```

## API Reference

### Library

| Method | Description |
|--------|-------------|
| `init()` | Initialize the library |

## Related Packages

This package is part of the Zovo extension utilities collection:

- [ext-storage-local](https://github.com/theluckystrike/ext-storage-local) - Local storage utilities
- [ext-storage-cache](https://github.com/theluckystrike/ext-storage-cache) - Cache storage utilities
- [ext-chrome-storage-sync](https://github.com/theluckystrike/ext-chrome-storage-sync) - Chrome storage sync wrapper

## Contributing

Contributions are welcome! Please follow these steps:

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/storage-improvement`
3. **Make** your changes
4. **Test** your changes: `npm test`
5. **Commit** your changes: `git commit -m 'Add new feature'`
6. **Push** to the branch: `git push origin feature/storage-improvement`
7. **Submit** a Pull Request

### Development Setup

```bash
# Clone the repository
git clone https://github.com/theluckystrike/ext-storage-sync.git
cd ext-storage-sync

# Install dependencies
npm install

# Run tests
npm test

# Build
npm run build
```

## Built by Zovo

Part of the [Zovo](https://zovo.one) developer tools family — privacy-first Chrome extensions built by developers, for developers.

## See Also

### Related Zovo Repositories

- [zovo-extension-template](https://github.com/theluckystrike/zovo-extension-template) - Boilerplate for building privacy-first Chrome extensions
- [zovo-types-webext](https://github.com/theluckystrike/zovo-types-webext) - Comprehensive TypeScript type definitions for browser extensions
- [zovo-permissions-scanner](https://github.com/theluckystrike/zovo-permissions-scanner) - Privacy scanner for Chrome extensions
- [zovo-indexer](https://github.com/theluckystrike/zovo-indexer) - Indexing service for Zovo extensions

### Zovo Chrome Extensions

- [Zovo Tab Manager](https://chrome.google.com/webstore/detail/zovo-tab-manager) - Manage tabs efficiently
- [Zovo Focus](https://chrome.google.com/webstore/detail/zovo-focus) - Block distractions
- [Zovo Permissions Scanner](https://chrome.google.com/webstore/detail/zovo-permissions-scanner) - Check extension privacy grades

Visit [zovo.one](https://zovo.one) for more information.

## License

MIT - [Zovo](https://zovo.one)

---

*Built by developers, for developers. No compromises on privacy.*
