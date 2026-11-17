---
title: "Clase TimelineCollection"
linktitle: "TimelineCollection"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase TimelineCollection. Encapsula el objeto que representa timelinecollection en Go."
type: docs
weight: 200
url: /es/go-cpp/timelinecollection/
---

## TimelineCollection class

Specifies the collection of all the <see cref="Timeline"/> objects on the worksheet.It was supported since Excel 2013.

```go

type TimelineCollection struct  {
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
| [Get_Int](./get_int/) | Obtiene el Timeline por índice. |
| [Get_String](./get_string/) | Obtiene el Timeline por el nombre del Timeline. |
| [Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | Agregar una nueva línea de tiempo usando PivotTable como origen de datos |
| [Add_PivotTable_String_String](./add_pivottable_string_string/) | Agregar una nueva línea de tiempo usando PivotTable como origen de datos |
| [Add_PivotTable_Int_Int_Int](./add_pivottable_int_int_int/) | Agregar una nueva línea de tiempo usando PivotTable como origen de datos |
| [Add_PivotTable_String_Int](./add_pivottable_string_int/) | Agregar una nueva línea de tiempo usando PivotTable como origen de datos |
| [Add_PivotTable_Int_Int_PivotField](./add_pivottable_int_int_pivotfield/) | Agregar una nueva línea de tiempo usando PivotTable como origen de datos |
| [Add_PivotTable_String_PivotField](./add_pivottable_string_pivotfield/) | Agregar una nueva línea de tiempo usando PivotTable como origen de datos |
| [GetCount](./getcount/) | Gets the number of elements contained in the instance. |
