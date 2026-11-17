---
title: "Clase RowCollection"
linktitle: "RowCollection"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase RowCollection. Encapsula el objeto que representa rowcollection en Go."
type: docs
weight: 200
url: /es/go-cpp/rowcollection/
---

## RowCollection class

Collects the <see cref="Row"/> objects that represent the individual rows in a worksheet.

```go

type RowCollection struct  {
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
| [GetCount](./getcount/) | Obtiene el número de filas en esta colección. |
| [GetEnumerator](./getenumerator/) | Obtiene un enumerador que recorre las filas de esta colección |
| [GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Obtiene un enumerador que recorre las filas de esta colección |
| [GetRowByIndex](./getrowbyindex/) | Obtiene el objeto fila por la posición en la lista. |
| [Get](./get/) | Obtiene un objeto Row por el índice de fila dado. El objeto Row del índice de fila dado se instanciará si no existe previamente. |
| [Clear](./clear/) | Borra todas las filas y celdas. |
| [RemoveAt](./removeat/) | Elimina el elemento de fila en el índice (posición) especificado en esta colección. |
