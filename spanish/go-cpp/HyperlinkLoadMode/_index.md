---
title: "Enumeración HyperlinkLoadMode"
linktitle: "HyperlinkLoadMode"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Enumeración HyperlinkLoadMode. Encapsula el objeto que representa hyperlinkloadmode en Go."
type: docs
weight: 200
url: /es/go-cpp/hyperlinkloadmode/
---

## HyperlinkLoadMode Enum

Specifies how hyperlinks are handled when loading HTML.

```go

type HyperlinkLoadMode int32


```

## Fields

| Field | Description |
| --- | --- |
| [Normal](./normal/) | Solo se carga el primer hipervínculo en una celda, los siguientes se ignoran. |
| [AllowMultiple](./allowmultiple/) | Todos los hipervínculos en una celda se añaden a <see cref="Worksheet.Hyperlinks"/>.Tenga en cuenta que MS Excel solo admite un hipervínculo por celda,por lo que esta opción puede generar archivos que Excel no pueda renderizar completamente. |
