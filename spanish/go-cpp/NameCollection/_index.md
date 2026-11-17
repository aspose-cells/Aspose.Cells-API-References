---
title: "Clase NameCollection"
linktitle: "NameCollection"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase NameCollection. Encapsula el objeto que representa namecollection en Go."
type: docs
weight: 200
url: /es/go-cpp/namecollection/
---

## NameCollection class

Represents a collection of all the <see cref="Name"/> objects in the spreadsheet.

```go

type NameCollection struct  {
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
| [Add](./add/) | Define un nuevo nombre. |
| [Get_Int](./get_int/) | Obtiene el elemento Name en el índice especificado. |
| [Filter](./filter/) | Obtiene todos los nombres definidos por alcance. |
| [Get_String](./get_string/) | Obtiene el elemento Name con el nombre especificado. |
| [Remove_stringArray](./remove_stringarray/) | Elimina una matriz de nombres |
| [Remove_String](./remove_string/) | Elimina el nombre. |
| [RemoveAt](./removeat/) | Elimina el nombre en el índice específico. |
| [Clear](./clear/) | Elimina todos los nombres definidos que no están referenciados por las fórmulas y la fuente de datos. Si el nombre definido está referenciado, solo establecemos Name.ReferTo como nulo y los ocultamos. |
| [RemoveDuplicateNames](./removeduplicatenames/) | Elimina los nombres definidos duplicados |
| [Sort](./sort/) | Ordena los nombres definidos. |
| [GetCount](./getcount/) | Gets the number of elements contained in the instance. |
