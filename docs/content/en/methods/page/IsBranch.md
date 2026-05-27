---
title: IsBranch
description: Reports whether the given page is a branch page.
categories: []
keywords: []
params:
  functions_and_methods:
    returnType: bool
    signatures: [PAGE.IsBranch]
---

The `IsBranch` method on a `Page` object returns `true` if the [page kind](g) is `home`, `section`, `taxonomy`, or `term`.

```text
content/
├── books/
│   ├── book-1/
│   │   └── index.md    <-- kind = page
│   ├── book-2.md       <-- kind = page
│   └── _index.md       <-- kind = section
├── tags
│   ├── fiction
│   │   └── _index.md   <-- kind = term
│   └── _index.md       <-- kind = taxonomy
└── _index.md           <-- kind = home
```

```go-html-template
{{ .IsBranch }}
```
