---
title: GridCells
second_title: Referencia de API de Aspose.Cells para .NET
description: Encapsula una colección deCell objetos.
type: docs
weight: 190
url: /es/net/aspose.cells.gridweb.data/gridcells/
---
## GridCells class

Encapsula una colección deCell objetos.

```csharp
public class GridCells : IEnumerable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Columns](../../aspose.cells.gridweb.data/gridcells/columns) { get; } |  |
| [Count](../../aspose.cells.gridweb.data/gridcells/count) { get; } | Obtiene el número de celdas. |
| [FirstCell](../../aspose.cells.gridweb.data/gridcells/firstcell) { get; } |  |
| [Item](../../aspose.cells.gridweb.data/gridcells/item) { get; } | ObtieneCell elemento dentro de la hoja de trabajo (3 indexers) |
| [LastCell](../../aspose.cells.gridweb.data/gridcells/lastcell) { get; } |  |
| [MaxColumn](../../aspose.cells.gridweb.data/gridcells/maxcolumn) { get; } | Índice de columna máximo de celda que contiene datos o estilo. |
| [MaxDataColumn](../../aspose.cells.gridweb.data/gridcells/maxdatacolumn) { get; } |  |
| [MaxDataRow](../../aspose.cells.gridweb.data/gridcells/maxdatarow) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/gridcells/maxrow) { get; } | Índice de fila máximo de celda que contiene datos o estilo. |
| [MergedCells](../../aspose.cells.gridweb.data/gridcells/mergedcells) { get; } | Obtiene la colección de celdas combinadas. |
| [MinColumn](../../aspose.cells.gridweb.data/gridcells/mincolumn) { get; } |  |
| [MinDataColumn](../../aspose.cells.gridweb.data/gridcells/mindatacolumn) { get; } |  |
| [MinDataRow](../../aspose.cells.gridweb.data/gridcells/mindatarow) { get; } |  |
| [MinRow](../../aspose.cells.gridweb.data/gridcells/minrow) { get; } |  |
| [RowEnumerator](../../aspose.cells.gridweb.data/gridcells/rowenumerator) { get; } | Obtiene las filas enumerator |
| [Rows](../../aspose.cells.gridweb.data/gridcells/rows) { get; } |  |
| [StandardHeight](../../aspose.cells.gridweb.data/gridcells/standardheight) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de puntos. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridcells/standardheightpixels) { get; set; } | Obtiene o establece el alto de fila predeterminado en esta hoja de cálculo, en unidades de píxeles. |
| [StandardWidth](../../aspose.cells.gridweb.data/gridcells/standardwidth) { get; set; } | Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de caracteres. |
| [StandardWidthInch](../../aspose.cells.gridweb.data/gridcells/standardwidthinch) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.gridweb.data/gridcells/standardwidthpixels) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/gridcells/clear)() | Limpia todas las celdas de la colección. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents#clearcontents)(GridCellArea) | Borra el contenido de un rango. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents#clearcontents_1)(int, int, int, int) | Borra el contenido de un rango. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats#clearformats)(GridCellArea) | Borra el formato de un rango. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats#clearformats_1)(int, int, int, int) | Borra el formato de un rango. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange#clearrange)(GridCellArea) | Borra el contenido y el formato de un rango. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange#clearrange_1)(int, int, int, int) | Borra el contenido y el formato de un rango. |
| [CopyColumn](../../aspose.cells.gridweb.data/gridcells/copycolumn)(GridCells, int, int) | Copia datos y formatos de una columna completa. |
| [CopyColumns](../../aspose.cells.gridweb.data/gridcells/copycolumns)(GridCells, int, int, int) | Copia datos y formatos de una columna completa. |
| [CopyRow](../../aspose.cells.gridweb.data/gridcells/copyrow)(GridCells, int, int) | Copia datos y formatos de una fila completa. |
| [CopyRows](../../aspose.cells.gridweb.data/gridcells/copyrows)(GridCells, int, int, int) | Copia datos y formatos de algunas filas completas. |
| [DeleteBlankColumns](../../aspose.cells.gridweb.data/gridcells/deleteblankcolumns)() | Eliminar todas las columnas en blanco que no contengan ningún dato. |
| [DeleteBlankRows](../../aspose.cells.gridweb.data/gridcells/deleteblankrows)() | Eliminar todas las filas en blanco que no contienen ningún dato. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn#deletecolumn)(int) | Elimina una columna. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn#deletecolumn_1)(int, bool) | Elimina una columna. |
| [DeleteColumns](../../aspose.cells.gridweb.data/gridcells/deletecolumns)(int, int, bool) | Elimina varias columnas. |
| [DeleteRange](../../aspose.cells.gridweb.data/gridcells/deleterange)(int, int, int, int, GridShiftType) | Elimina un rango de celdas y desplaza celdas según la opción de desplazamiento. |
| [DeleteRow](../../aspose.cells.gridweb.data/gridcells/deleterow)(int) | Elimina una fila. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows#deleterows)(int, int) | Elimina varias filas. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows#deleterows_1)(int, int, bool) | Elimina varias filas en la hoja de cálculo. |
| [Export](../../aspose.cells.gridweb.data/gridcells/export)(int, int, int, int, bool, bool) | Exporta datos en la colección Cells de una WebWorksheet a un nuevo objeto DataTable |
| [ExportArray](../../aspose.cells.gridweb.data/gridcells/exportarray)(int, int, int, int) | Exporta datos en elCellscolección a un objeto de matriz de dos dimensiones. |
| [GetCell](../../aspose.cells.gridweb.data/gridcells/getcell)(int, int) | Obtiene elCell elemento o nulo en el índice de fila de celda y el índice de columna especificados. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/gridcells/getcolumnwidth)(int) | Obtiene el ancho de la columna especificada |
| [GetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthinch)(int) | Obtiene el ancho de la columna especificada, en unidades de pulgadas. |
| [GetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthpixel)(int) | Obtiene el ancho de la columna especificada, en unidades de píxel. |
| [GetEnumerator](../../aspose.cells.gridweb.data/gridcells/getenumerator)() | Obtiene las filas enumerator |
| [GetRow](../../aspose.cells.gridweb.data/gridcells/getrow)(int) | Obtiene elRow elemento o en la fila de celda especificada index. |
| [GetRowHeight](../../aspose.cells.gridweb.data/gridcells/getrowheight)(int) | Obtiene la altura de una fila especificada. |
| [GetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/getrowheightinch)(int) | Obtiene la altura de una fila especificada en unidades de pulgadas. |
| [GetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/getrowheightpixel)(int) | Obtiene la altura de una fila especificada en unidades de píxel. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/getrowoutlinelevel)(int) | Obtiene el nivel de esquema de la fila. |
| [GetViewColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getviewcolumnwidthpixel)(int) | Obtener el ancho en diferente tipo de vista. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns#groupcolumns)(int, int) | Agrupa columnas. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns#groupcolumns_1)(int, int, bool) | Agrupa columnas. |
| [GroupRows](../../aspose.cells.gridweb.data/gridcells/grouprows)(int, int) | Agrupa filas. |
| [HideColumn](../../aspose.cells.gridweb.data/gridcells/hidecolumn)(int) | Oculta una columna. |
| [HideRow](../../aspose.cells.gridweb.data/gridcells/hiderow)(int) | Oculta una fila. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn#insertcolumn)(int) | Inserta una nueva columna en la hoja de cálculo. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn#insertcolumn_1)(int, bool) | Inserta una nueva columna en la hoja de cálculo. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns#insertcolumns)(int, int) | Inserta algunas columnas en la hoja de trabajo. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns#insertcolumns_1)(int, int, bool) | Inserta algunas columnas en la hoja de trabajo. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange#insertrange)(GridCellArea, GridShiftType) | Inserta un rango de celdas y desplaza celdas según la opción de desplazamiento. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange#insertrange_1)(GridCellArea, int, GridShiftType, bool) | Inserta un rango de celdas y desplaza celdas según la opción de desplazamiento. |
| [InsertRow](../../aspose.cells.gridweb.data/gridcells/insertrow)(int) | Inserta una nueva fila en la hoja de cálculo. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows#insertrows)(int, int) | Inserta varias filas en la hoja de trabajo. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows#insertrows_1)(int, int, bool) | Inserta varias filas en la hoja de trabajo. |
| [IsBlankColumn](../../aspose.cells.gridweb.data/gridcells/isblankcolumn)(int) | Comprueba si la columna dada está en blanco (no contiene ningún dato). |
| [IsColumnHidden](../../aspose.cells.gridweb.data/gridcells/iscolumnhidden)(int) | Comprueba si una columna en el índice dado está oculta. |
| [IsRowHidden](../../aspose.cells.gridweb.data/gridcells/isrowhidden)(int) | Comprueba si una fila en el índice dado está oculta. |
| [Merge](../../aspose.cells.gridweb.data/gridcells/merge)(int, int, int, int) | Combina un rango específico de celdas en una sola celda. |
| [MoveRange](../../aspose.cells.gridweb.data/gridcells/moverange)(GridCellArea, int, int) | Mueve el rango. |
| [RemoveFormulas](../../aspose.cells.gridweb.data/gridcells/removeformulas)() | Elimina todas las fórmulas y las reemplaza con el valor de la fórmula. |
| [SetBorders](../../aspose.cells.gridweb.data/gridcells/setborders)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Establece los bordes de un rango de celdas. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/gridcells/setcolumnwidth)(int, double) | Establece el ancho de la columna especificada. |
| [SetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthinch)(int, double) | Establece el ancho de columna en unidades de pulgadas. |
| [SetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthpixel)(int, int) | Establece el ancho de columna en unidades de píxeles. |
| [SetRowHeight](../../aspose.cells.gridweb.data/gridcells/setrowheight)(int, double) | Establece la altura de la fila especificada. |
| [SetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/setrowheightinch)(int, double) | Establece la altura de fila en unidades de pulgadas. |
| [SetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/setrowheightpixel)(int, int) | Establece la altura de la fila en unidades de píxeles. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/setrowoutlinelevel)(int, int) | Establece el nivel de contorno de la fila. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle#setstyle_1)(string, GridTableItemStyle) | Establece el estilo en un rango específico de celdas. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle#setstyle)(int, int, int, int, GridTableItemStyle) | Establece el estilo en un rango específico de celdas. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort#sort)(int, int, int, int, int, bool, bool, bool) | Ordena los datos ascendentes/descendentes de arriba a abajo en un rango de una hoja de trabajo por índice de columna especificado. Ordena los datos ascendentes/descendentes de izquierda a derecha en un rango de una hoja de trabajo por índice de fila especificado. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) |  |
| [UngroupColumns](../../aspose.cells.gridweb.data/gridcells/ungroupcolumns)(int, int) | Desagrupa columnas. |
| [UngroupRows](../../aspose.cells.gridweb.data/gridcells/ungrouprows)(int, int) | Desagrupa filas. |
| [UnhideColumn](../../aspose.cells.gridweb.data/gridcells/unhidecolumn)(int, double) | Muestra una columna |
| [UnhideRow](../../aspose.cells.gridweb.data/gridcells/unhiderow)(int) | Muestra una fila. |
| [UnMerge](../../aspose.cells.gridweb.data/gridcells/unmerge)(int, int, int, int) | Separa un rango específico de celdas combinadas. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/gridcells/cellindextoname)(int, int) | Obtiene el nombre de la celda según sus índices de fila y columna. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/gridcells/cellnametoindex)(string, out int, out int) | Obtiene los índices de fila y columna de celda según su nombre |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/gridcells/columnindextoname)(int) | Obtiene el nombre de la columna según el índice de la columna. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/gridcells/columnnametoindex)(string) | Obtiene el índice de la columna según el nombre de la columna. |

### Ver también

* espacio de nombres [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* asamblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
