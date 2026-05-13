# @onlyoffice/doceditor-types

TypeScript type definitions for the [ONLYOFFICE Document Editor API](https://api.onlyoffice.com/docs/docs-api/usage-api/config/).

Provides full IntelliSense, type checking, and inline documentation for:

- **Config** — the editor initialization config (`Config`, `ConfigNormal`, `ConfigEmbedded`)
- **DocEditor** — typed method signatures for the editor instance
- **Events** — all editor event callback types
- **Permissions, Customization, Document Info** — every nested config section

## Install

```bash
npm install @onlyoffice/doceditor-types
```

## Usage

```typescript
import type { Config, DocEditor } from "@onlyoffice/doceditor-types";

const config: Config = {
  documentType: "word",
  document: {
    fileType: "docx",
    key: "unique-key",
    title: "Example.docx",
    url: "https://example.com/document.docx",
  },
  editorConfig: {
    callbackUrl: "https://example.com/callback",
    lang: "en",
  },
};

// Pass to DocsAPI.DocEditor constructor
const editor = new DocsAPI.DocEditor("placeholder", config);
```

## Versioning

This package version tracks the ONLYOFFICE Docs Server version.

| Package version | Docs Server version |
| --------------- | ------------------- |
| 9.3.1           | 9.3.1               |

## Documentation

Full API reference: <https://api.onlyoffice.com/docs/docs-api/usage-api/config/>

## License

[Apache-2.0](LICENSE)
