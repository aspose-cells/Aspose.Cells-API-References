---
title: "Clase DataSorter"
linktitle: "DataSorter"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "DataSorter class. Encapsula el objeto que representa datasorter en Go."
type: docs
weight: 200
url: /es/go-cpp/datasorter/
---

## DataSorter class

Summary description for DataSorter.

```go

type DataSorter struct  {
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
| [GetKeys](./getkeys/) | Obtiene la lista de claves del data sorter. |
| [Clear](./clear/) | Borrar todas las configuraciones. |
| [GetHasHeaders](./gethasheaders/) | Representa si el rango tiene encabezados. |
| [SetHasHeaders](./sethasheaders/) | Representa si el rango tiene encabezados. |
| [AddKey_Int_SortOrder](./addkey_int_sortorder/) | Agrega el índice de columna ordenada y el orden de clasificación. |
| [AddKey_Int_SortOrder_String](./addkey_int_sortorder_string/) | Agrega el índice de columna ordenada y el orden de clasificación con una lista de orden personalizada. |
| [AddColorKey](./addcolorkey/) | Agrega la clave de ordenación por color. |
| [AddKey_Int_SortOnType_SortOrder_Object](./addkey_int_sortontype_sortorder_object/) | Agrega el índice de columna ordenada y el orden de clasificación con una lista de orden personalizada. |
| [AddKey_Int_SortOrder_stringArray](./addkey_int_sortorder_stringarray/) | Agrega el índice de columna ordenada y el orden de clasificación con una lista de orden personalizada. |
| [GetKey1](./getkey1/) | Representa el índice de la primera columna ordenada(posición absoluta, la columna A es 0, B es 1, ...). |
| [SetKey1](./setkey1/) | Representa el índice de la primera columna ordenada(posición absoluta, la columna A es 0, B es 1, ...). |
| [GetOrder1](./getorder1/) | Representa el orden de clasificación de la primera clave. |
| [SetOrder1](./setorder1/) | Representa el orden de clasificación de la primera clave. |
| [GetKey2](./getkey2/) | Representa el índice de la segunda columna ordenada(posición absoluta, la columna A es 0, B es 1, ...). |
| [SetKey2](./setkey2/) | Representa el índice de la segunda columna ordenada(posición absoluta, la columna A es 0, B es 1, ...). |
| [GetOrder2](./getorder2/) | Representa el orden de clasificación de la segunda clave. |
| [SetOrder2](./setorder2/) | Representa el orden de clasificación de la segunda clave. |
| [GetKey3](./getkey3/) | Representa el índice de la tercera columna ordenada(posición absoluta, la columna A es 0, B es 1, ...). |
| [SetKey3](./setkey3/) | Representa el índice de la tercera columna ordenada(posición absoluta, la columna A es 0, B es 1, ...). |
| [GetOrder3](./getorder3/) | Representa el orden de clasificación de la tercera clave. |
| [SetOrder3](./setorder3/) | Representa el orden de clasificación de la tercera clave. |
| [GetSortLeftToRight](./getsortlefttoright/) | True significa que la orientación de ordenación es de izquierda a derecha.False significa que la orientación de ordenación es de arriba a abajo.El valor predeterminado es false. |
| [SetSortLeftToRight](./setsortlefttoright/) | True significa que la orientación de ordenación es de izquierda a derecha.False significa que la orientación de ordenación es de arriba a abajo.El valor predeterminado es false. |
| [GetCaseSensitive](./getcasesensitive/) | Obtiene y establece si la comparación de cadenas distingue mayúsculas y minúsculas. |
| [SetCaseSensitive](./setcasesensitive/) | Obtiene y establece si la comparación de cadenas distingue mayúsculas y minúsculas. |
| [GetSortAsNumber](./getsortasnumber/) | Indica si se ordena cualquier cosa que parezca un número. |
| [SetSortAsNumber](./setsortasnumber/) | Indica si se ordena cualquier cosa que parezca un número. |
| [Sort_Cells_Int_Int_Int_Int](./sort_cells_int_int_int_int/) | Ordena los datos del área. |
| [Sort_Cells_CellArea](./sort_cells_cellarea/) | Ordena los datos del área. |
| [Sort](./sort/) | Ordena los datos en el rango. |
