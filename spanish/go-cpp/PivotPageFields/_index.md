---
title: "Clase PivotPageFields"
linktitle: "PivotPageFields"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "PivotPageFields class. Encapsula el objeto que representa pivotpagefields en Go."
type: docs
weight: 200
url: /es/go-cpp/pivotpagefields/
---

## PivotPageFields class

Represents the pivot page itemsif the pivot table data source is consolidation ranges.It only can contain up to 4 items.

```go

type PivotPageFields struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
| [NewPivotPageFields](./newpivotpagefields/) | Representa los elementos del campo de página pivote. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [AddPageField](./addpagefield/) | Agrega un campo de página. |
| [GetPageFieldCount](./getpagefieldcount/) | Obtiene el número de campos de página. |
| [AddIdentify](./addidentify/) | Establece qué etiqueta de elemento en cada campo de página usar para identificar el rango de datos. El pageItemIndex.Length debe ser igual a PageFieldCount, así que por favor agregue primero el campo de página. |
