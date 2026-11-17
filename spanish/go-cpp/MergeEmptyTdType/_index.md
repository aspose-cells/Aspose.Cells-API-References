---
title: "Enumeración MergeEmptyTdType"
linktitle: "MergeEmptyTdType"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Enumeración MergeEmptyTdType. Encapsula el objeto que representa mergeemptytdtype en Go."
type: docs
weight: 200
url: /es/go-cpp/mergeemptytdtype/
---

## MergeEmptyTdType Enum

Represents the merge type for an empty TD element when exporting a file to HTML.

```go

type MergeEmptyTdType int32


```

## Fields

| Field | Description |
| --- | --- |
| [Default](./default/) | Mostrar como MS Excel. |
| [None](./none/) | Los elementos TD vacíos no se fusionarán al exportar el archivo a HTML. Esto generará un archivo HTML significativamente más grande. |
| [MergeForcely](./mergeforcely/) | Fusionar forzadamente los elementos TD vacíos al exportar el archivo a HTML. El tamaño del archivo HTML se reducirá significativamente al establecer el valor en verdadero. Si desea importar el archivo HTML a Excel o exportar líneas de cuadrícula perfectas al guardar el archivo en HTML, mantenga el valor predeterminado. |
