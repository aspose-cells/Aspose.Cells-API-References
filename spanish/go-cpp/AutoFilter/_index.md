---
title: "Clase AutoFilter"
linktitle: "AutoFilter"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase AutoFilter. Encapsula el objeto que representa el autofiltro en Go."
type: docs
weight: 200
url: /es/go-cpp/autofilter/
---

## AutoFilter class

Represents autofiltering for the specified worksheet.

```go

type AutoFilter struct  {
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
| [GetSorter](./getsorter/) | Obtiene el clasificador de datos. |
| [SetRange_Int_Int_Int](./setrange_int_int_int/) | Establece el rango al que se aplica el AutoFilter especificado. |
| [GetCellArea](./getcellarea/) | Obtiene el CellArea donde se aplica este AutoFilter. |
| [GetCellArea_Bool](./getcellarea_bool/) | Obtiene el Aspose.Cells.CellArea donde se aplica el AutoFilter especificado. |
| [GetRange](./getrange/) | Representa el rango al que se aplica el AutoFilter especificado. |
| [SetRange_String](./setrange_string/) | Representa el rango al que se aplica el AutoFilter especificado. |
| [AddFilter](./addfilter/) | Agrega un filtro para una columna de filtro. |
| [AddDateFilter](./adddatefilter/) | Agrega un filtro de fecha. |
| [RemoveDateFilter](./removedatefilter/) | Elimina un filtro de fecha. |
| [RemoveFilter_Int_String](./removefilter_int_string/) | Elimina un filtro para una columna de filtro. |
| [Filter](./filter/) | Filtra una lista con criterios especificados. |
| [FilterTop10](./filtertop10/) | Filtra los 10 elementos principales de la lista. |
| [Dynamic_Filter](./dynamic_filter/) | Agrega un filtro dinámico. |
| [AddFontColorFilter](./addfontcolorfilter/) | Agrega un filtro de color de fuente. |
| [AddFillColorFilter](./addfillcolorfilter/) | Agrega un filtro de color de relleno. |
| [AddIconFilter](./addiconfilter/) | Agrega un filtro de ícono. |
| [MatchBlanks](./matchblanks/) | Coincide con todas las celdas en blanco de la lista. |
| [MatchNonBlanks](./matchnonblanks/) | Coincide con todas las celdas que no están en blanco de la lista. |
| [Custom_Int_FilterOperatorType_Object](./custom_int_filteroperatortype_object/) | Filtra una lista con un criterio personalizado. |
| [Custom_Int_FilterOperatorType_Object_Bool_FilterOperatorType_Object](./custom_int_filteroperatortype_object_bool_filteroperatortype_object/) | Filters a list with custom criteria. |
| [ShowAll](./showall/) | Desocultar todas las filas. |
| [RemoveFilter_Int](./removefilter_int/) | Eliminar el filtro específico. |
| [Refresh](./refresh/) | Actualizar los autofiltros para ocultar o desocultar las filas. |
| [Refresh_Bool](./refresh_bool/) | Obtiene los índices de todas las filas ocultas. |
| [GetShowFilterButton](./getshowfilterbutton/) | Indicates whether the AutoFilter button for this column is visible. |
| [SetShowFilterButton](./setshowfilterbutton/) | Indicates whether the AutoFilter button for this column is visible. |
| [GetFilterColumns](./getfiltercolumns/) | Obtiene la colección de las columnas de filtro. |
