---
title: "Clase GridCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridDesktop.Data.GridCells. Encapsula una colección de objetos Cell"
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridcells/
---
## GridCells class

Encapsula una colección de objetos Cell.

```csharp
public class GridCells : IEnumerable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Columns](../../aspose.cells.griddesktop.data/gridcells/columns/) { get; } |  |
| [Count](../../aspose.cells.griddesktop.data/gridcells/count/) { get; } | Obtiene el número de celdas. |
| [FirstCell](../../aspose.cells.griddesktop.data/gridcells/firstcell/) { get; } | Obtiene la primera celda en esta hoja de cálculo. |
| [Item](../../aspose.cells.griddesktop.data/gridcells/item/) { get; } | Obtiene el elemento [`GridCell`](../gridcell/) en el índice de fila y columna de celda especificados. (2 indexadores) |
| [LastCell](../../aspose.cells.griddesktop.data/gridcells/lastcell/) { get; } | Obtiene la última celda en esta hoja de cálculo. |
| [MaxColumn](../../aspose.cells.griddesktop.data/gridcells/maxcolumn/) { get; } | Índice máximo de columna de la celda que contiene datos o estilo. |
| [MaxDataColumn](../../aspose.cells.griddesktop.data/gridcells/maxdatacolumn/) { get; } | Índice máximo de columna de la celda que contiene datos. |
| [MaxDataRow](../../aspose.cells.griddesktop.data/gridcells/maxdatarow/) { get; } | Índice máximo de fila de la celda que contiene datos. |
| [MaxRow](../../aspose.cells.griddesktop.data/gridcells/maxrow/) { get; } | Índice máximo de fila de la celda que contiene datos o estilo. |
| [MergedCells](../../aspose.cells.griddesktop.data/gridcells/mergedcells/) { get; } | Obtiene la colección de celdas combinadas. |
| [MinColumn](../../aspose.cells.griddesktop.data/gridcells/mincolumn/) { get; } | Índice mínimo de columna de esas celdas que han sido instanciadas en la colección (no incluye la columna donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda en ella). |
| [MinDataColumn](../../aspose.cells.griddesktop.data/gridcells/mindatacolumn/) { get; } | Índice mínimo de columna de la celda que contiene datos. |
| [MinDataRow](../../aspose.cells.griddesktop.data/gridcells/mindatarow/) { get; } | Índice de fila mínimo de la celda que contiene datos. |
| [MinRow](../../aspose.cells.griddesktop.data/gridcells/minrow/) { get; } | Índice de fila mínimo de la celda que contiene datos o estilo. |
| [RowEnumerator](../../aspose.cells.griddesktop.data/gridcells/rowenumerator/) { get; } | Obtiene el enumerador de filas |
| [Rows](../../aspose.cells.griddesktop.data/gridcells/rows/) { get; } | Obtiene la colección de objetos [`GridRow`](../gridrow/) que representan las filas individuales en esta hoja de cálculo. |
| [StandardHeight](../../aspose.cells.griddesktop.data/gridcells/standardheight/) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de puntos. |
| [StandardHeightPixels](../../aspose.cells.griddesktop.data/gridcells/standardheightpixels/) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de píxeles. |
| [StandardWidth](../../aspose.cells.griddesktop.data/gridcells/standardwidth/) { get; set; } | Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de caracteres. |
| [StandardWidthInch](../../aspose.cells.griddesktop.data/gridcells/standardwidthinch/) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.griddesktop.data/gridcells/standardwidthpixels/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CheckCell](../../aspose.cells.griddesktop.data/gridcells/checkcell/)(int, int) | Obtiene el elemento [`GridCell`](../gridcell/) o null en el índice de fila y columna de celda especificados. |
| [CheckRow](../../aspose.cells.griddesktop.data/gridcells/checkrow/)(int) | Obtiene el elemento [`GridRow`](../gridrow/) o null en el índice de fila de celda especificado. |
| [Clear](../../aspose.cells.griddesktop.data/gridcells/clear/)() | Borra todas las celdas de la colección. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | Borra el contenido de un rango. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | Borra el contenido de un rango. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats)(GridCellArea) | Borra el formato de un rango. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | Borra el formato de un rango. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange)(GridCellArea) | Borra el contenido y el formato de un rango. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | Borra el contenido y el formato de un rango. |
| [CopyColumn](../../aspose.cells.griddesktop.data/gridcells/copycolumn/)(GridCells, int, int) | Copia los datos y formatos de una columna completa. |
| [CopyColumns](../../aspose.cells.griddesktop.data/gridcells/copycolumns/)(GridCells, int, int, int) | Copia los datos y formatos de una columna completa. |
| [CopyRow](../../aspose.cells.griddesktop.data/gridcells/copyrow/)(GridCells, int, int) | Copia los datos y formatos de una fila completa. |
| [CopyRows](../../aspose.cells.griddesktop.data/gridcells/copyrows/)(GridCells, int, int, int) | Copia los datos y formatos de varias filas completas. |
| [DeleteBlankColumns](../../aspose.cells.griddesktop.data/gridcells/deleteblankcolumns/)() | Elimina todas las columnas en blanco que no contengan ningún dato. |
| [DeleteBlankRows](../../aspose.cells.griddesktop.data/gridcells/deleteblankrows/)() | Elimina todas las filas en blanco que no contienen datos. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn)(int) | Elimina una columna. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | Elimina una columna. |
| [DeleteColumns](../../aspose.cells.griddesktop.data/gridcells/deletecolumns/)(int, int, bool) | Elimina varias columnas. |
| [DeleteRow](../../aspose.cells.griddesktop.data/gridcells/deleterow/)(int) | Elimina una fila. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows)(int, int) | Elimina varias filas. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | Elimina varias filas en la hoja de cálculo. |
| [GetCellStyle](../../aspose.cells.griddesktop.data/gridcells/getcellstyle/)(int, int) | Obtiene el estilo de la celda dada. |
| [GetColumn](../../aspose.cells.griddesktop.data/gridcells/getcolumn/)(int) | Obtiene el elemento [`GridColumn`](../gridcolumn/) en el índice de columna de celda especificado. |
| [GetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidth/)(int) | Obtiene el ancho de la columna especificada |
| [GetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthinch/)(int) | Obtiene el ancho de la columna especificada, en unidades de pulgadas. |
| [GetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthpixel/)(int) | Obtiene el ancho de la columna especificada, en unidades de píxeles. |
| [GetEnumerator](../../aspose.cells.griddesktop.data/gridcells/getenumerator/)() | Obtiene el enumerador de filas |
| [GetRow](../../aspose.cells.griddesktop.data/gridcells/getrow/)(int) | Obtiene el elemento [`GridRow`](../gridrow/) en el índice de fila de celda especificado. |
| [GetRowHeight](../../aspose.cells.griddesktop.data/gridcells/getrowheight/)(int) | Obtiene la altura de una fila especificada. |
| [GetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/getrowheightinch/)(int) | Obtiene la altura de una fila especificada en unidades de pulgadas. |
| [GetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/getrowheightpixel/)(int) | Obtiene la altura de una fila especificada en unidades de píxel. |
| [GetViewColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getviewcolumnwidthpixel/)(int) | Obtiene el ancho en diferentes tipos de vista. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns)(int, int) | Agrupa columnas. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | Agrupa columnas. |
| [GroupRows](../../aspose.cells.griddesktop.data/gridcells/grouprows/)(int, int) | Agrupa filas. |
| [HideColumn](../../aspose.cells.griddesktop.data/gridcells/hidecolumn/)(int) | Oculta una columna. |
| [HideColumns](../../aspose.cells.griddesktop.data/gridcells/hidecolumns/)(int, int) | Oculta varias columnas. |
| [HideRow](../../aspose.cells.griddesktop.data/gridcells/hiderow/)(int) | Oculta una fila. |
| [HideRows](../../aspose.cells.griddesktop.data/gridcells/hiderows/)(int, int) | Oculta varias filas. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn)(int) | Inserta una nueva columna en la hoja de cálculo. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | Inserta una nueva columna en la hoja de cálculo. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns)(int, int) | Inserta algunas columnas en la hoja de cálculo. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | Inserta algunas columnas en la hoja de cálculo. |
| [InsertRow](../../aspose.cells.griddesktop.data/gridcells/insertrow/)(int) | Inserta una nueva fila en la hoja de cálculo. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows)(int, int) | Inserta varias filas en la hoja de cálculo. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | Inserta varias filas en la hoja de cálculo. |
| [IsBlankColumn](../../aspose.cells.griddesktop.data/gridcells/isblankcolumn/)(int) | Comprueba si la columna dada está vacía (no contiene datos). |
| [IsColumnHidden](../../aspose.cells.griddesktop.data/gridcells/iscolumnhidden/)(int) | Comprueba si una columna en el índice dado está oculta. |
| [IsRowHidden](../../aspose.cells.griddesktop.data/gridcells/isrowhidden/)(int) | Comprueba si una fila en el índice dado está oculta. |
| [Merge](../../aspose.cells.griddesktop.data/gridcells/merge/)(int, int, int, int) | Fusiona un rango especificado de celdas en una sola celda. |
| [RemoveFormulas](../../aspose.cells.griddesktop.data/gridcells/removeformulas/)() | Elimina todas las fórmulas y las reemplaza con el valor de la fórmula. |
| [SetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidth/)(int, double) | Establece el ancho de la columna especificada. |
| [SetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthinch/)(int, double) | Establece el ancho de la columna en unidades de pulgadas. |
| [SetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthpixel/)(int, int) | Establece el ancho de la columna en unidades de píxeles. |
| [SetRowHeight](../../aspose.cells.griddesktop.data/gridcells/setrowheight/)(int, double) | Establece la altura de la fila especificada. |
| [SetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/setrowheightinch/)(int, double) | Establece la altura de la fila en unidades de pulgadas. |
| [SetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/setrowheightpixel/)(int, int) | Establece la altura de la fila en unidades de píxeles. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle)(CellRange, Style) | Establece el estilo a un rango especificado de celdas. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_2)(string, Style) | Establece el estilo a un rango especificado de celdas. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_1)(int, int, int, int, Style) | Establece el estilo a un rango especificado de celdas. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | Ordena los datos ascendente/descendente de arriba a abajo en un rango de una hoja de cálculo por el índice de columna especificado. Ordena los datos ascendente/descendente de izquierda a derecha en un rango de una hoja de cálculo por el índice de fila especificado. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) | Ordena los datos del área. |
| [SortAsNumber](../../aspose.cells.griddesktop.data/gridcells/sortasnumber/)(int, int, int, int, int[], SortOrder[], SortOrientation) | Ordena los datos del área (los datos de la columna clave deben ser numéricos). |
| [UngroupColumns](../../aspose.cells.griddesktop.data/gridcells/ungroupcolumns/)(int, int) | Desagrupa columnas. |
| [UngroupRows](../../aspose.cells.griddesktop.data/gridcells/ungrouprows/)(int, int) | Desagrupa filas. |
| [UnhideColumn](../../aspose.cells.griddesktop.data/gridcells/unhidecolumn/)(int, double) | Muestra una columna |
| [UnhideColumns](../../aspose.cells.griddesktop.data/gridcells/unhidecolumns/)(int, int, double) | Muestra varias columnas. |
| [UnhideRow](../../aspose.cells.griddesktop.data/gridcells/unhiderow/)(int, int) | Muestra una fila. |
| [UnhideRows](../../aspose.cells.griddesktop.data/gridcells/unhiderows/)(int, int, double) | Muestra las filas ocultas. |
| [UnMerge](../../aspose.cells.griddesktop.data/gridcells/unmerge/)(int, int, int, int) | Descombina un rango especificado de celdas combinadas. |
| static [CellIndexToName](../../aspose.cells.griddesktop.data/gridcells/cellindextoname/)(int, int) | Obtiene el nombre de la celda según sus índices de fila y columna. |
| static [CellNameToIndex](../../aspose.cells.griddesktop.data/gridcells/cellnametoindex/)(string, out int, out int) | Obtiene los índices de fila y columna de la celda según su nombre |
| static [ColumnIndexToName](../../aspose.cells.griddesktop.data/gridcells/columnindextoname/)(int) | Obtiene el nombre de la columna según el índice de columna. |
| static [ColumnNameToIndex](../../aspose.cells.griddesktop.data/gridcells/columnnametoindex/)(string) | Obtiene el índice de columna según el nombre de columna. |

### Ver también

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


