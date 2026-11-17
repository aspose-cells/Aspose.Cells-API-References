---
title: "Clase UnionRange"
linktitle: "UnionRange"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase UnionRange. Encapsula el objeto que representa unionrange en Go."
type: docs
weight: 200
url: /es/go-cpp/unionrange/
---

## UnionRange class

Represents union range.

```go

type UnionRange struct  {
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
| [GetFirstRow](./getfirstrow/) | Gets the index of the first row of the range. |
| [GetFirstColumn](./getfirstcolumn/) | Gets the index of the first column of the range. |
| [GetRowCount](./getrowcount/) | Gets the count of rows in the range. |
| [GetColumnCount](./getcolumncount/) | Gets the count of rows in the range. |
| [Merge](./merge/) | Combines a range of cells into a single cell. |
| [UnMerge](./unmerge/) | Unmerges merged cells of this range. |
| [PutValue](./putvalue/) | Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [GetValue](./getvalue/) | Obtiene y establece los valores del rango. |
| [SetValue](./setvalue/) | Obtiene y establece los valores del rango. |
| [GetName](./getname/) | Gets or sets the name of the range. |
| [SetName](./setname/) | Gets or sets the name of the range. |
| [GetRefersTo](./getrefersto/) | Gets the range's refers to. |
| [GetHasRange](./gethasrange/) | Indica si esto tiene rango. |
| [GetHyperlinks](./gethyperlinks/) | Gets all hyperlink in the range. |
| [SetStyle](./setstyle/) | Sets the style of the range. |
| [ApplyStyle](./applystyle/) | Applies formats for a whole range. |
| [Copy](./copy/) | Copying the range with paste special options. |
| [GetEnumerator](./getenumerator/) | Gets the enumerator for cells in this Range. |
| [GetCellCount](./getcellcount/) | Obtiene el recuento total de celdas en el rango. |
| [GetRangeCount](./getrangecount/) | Obtiene el recuento de los rangos. |
| [GetRanges](./getranges/) | Obtiene todos los rangos de unión. |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | Sets out line borders around a range of cells. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | Sets the outline borders around a range of cells with same border style and color. |
| [Intersect_String](./intersect_string/) | Se intersecta con otro rango. |
| [Intersect_UnionRange](./intersect_unionrange/) | Se intersecta con otro rango. |
| [Intersect_RangeArray](./intersect_rangearray/) | Se intersecta con otro rango. |
| [Union_String](./union_string/) | Unir otro rango. |
| [Union_UnionRange](./union_unionrange/) | Unir otro rango. |
| [Union_RangeArray](./union_rangearray/) | Unir los rangos. |
