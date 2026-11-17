---
title: "SplitPartInfo Clase"
linktitle: "SplitPartInfo"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase SplitPartInfo. Encapsula el objeto que representa splitpartinfo en Go."
type: docs
weight: 200
url: /es/go-cpp/splitpartinfo/
---

## SplitPartInfo class

Represents the information of one input/output for multiple inputs/outputs,such as current page to be rendered when converting spreadsheet to image.

```go

type SplitPartInfo struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [GetPartIndex](./getpartindex/) | Índice de la parte actual en la secuencia (base 0). -1 indica que no hay múltiples partes, por lo que el resultado es único. |
| [GetSheetIndex](./getsheetindex/) | Índice de la hoja donde se encuentra la parte actual. -1 indica que solo hay una hoja. |
| [GetSheetName](./getsheetname/) | Nombre de la hoja donde se encuentra la parte actual. |
