---
title: HyperlinkLoadMode Enum 
linktitle: HyperlinkLoadMode
second_title: Aspose.Cells for Go via C++ API Reference
description: 'HyperlinkLoadMode enum. Encapsulates the object that represents hyperlinkloadmode in Go.'
type: docs
weight: 200
url: /go-cpp/hyperlinkloadmode/
---

## HyperlinkLoadMode Enum

Specifies how hyperlinks are handled when loading HTML.

```go

type HyperlinkLoadMode int32


```

## Fields

| Field | Description |
| --- | --- |
|[Normal](./normal/) | Only the first hyperlink in a cell is loaded, subsequent ones are ignored. | 
|[AllowMultiple](./allowmultiple/) | All hyperlinks in a cell are added to <see cref="Worksheet.Hyperlinks"/>.Note that MS Excel itself supports only one hyperlink per cell,so this option may produce files that Excel cannot fully render. | 
