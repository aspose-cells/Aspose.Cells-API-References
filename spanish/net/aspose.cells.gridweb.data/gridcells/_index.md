---
title: "Clase GridCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.Data.GridCells. Encapsula una colección de objetos GridCell"
type: docs
url: /es/net/aspose.cells.gridweb.data/gridcells/
---
## GridCells class

Encapsula una colección de objetos [`GridCell`](../gridcell/).

```csharp
public class GridCells : IEnumerable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Columns](../../aspose.cells.gridweb.data/gridcells/columns/) { get; } | Obtiene la colección de objetos [`GridColumn`](../gridcolumn/) que representan las columnas individuales en esta hoja de cálculo. |
| [Count](../../aspose.cells.gridweb.data/gridcells/count/) { get; } | Obtiene el número de celdas. |
| [FirstCell](../../aspose.cells.gridweb.data/gridcells/firstcell/) { get; } | Obtiene la primera celda en esta hoja de cálculo. |
| [Item](../../aspose.cells.gridweb.data/gridcells/item/) { get; } | Obtiene el elemento [`GridCell`](../gridcell/) en el índice de fila y columna de celda especificados. (2 indexadores) |
| [LastCell](../../aspose.cells.gridweb.data/gridcells/lastcell/) { get; } | Obtiene la última celda en esta hoja de cálculo. |
| [MaxColumn](../../aspose.cells.gridweb.data/gridcells/maxcolumn/) { get; } | Índice máximo de columna de la celda que contiene datos o estilo. |
| [MaxDataColumn](../../aspose.cells.gridweb.data/gridcells/maxdatacolumn/) { get; } | Índice máximo de columna de la celda que contiene datos. |
| [MaxDataRow](../../aspose.cells.gridweb.data/gridcells/maxdatarow/) { get; } | Índice máximo de fila de la celda que contiene datos. |
| [MaxRow](../../aspose.cells.gridweb.data/gridcells/maxrow/) { get; } | Índice máximo de fila de la celda que contiene datos o estilo. |
| [MergedCells](../../aspose.cells.gridweb.data/gridcells/mergedcells/) { get; } | Obtiene la colección de celdas combinadas. |
| [MinColumn](../../aspose.cells.gridweb.data/gridcells/mincolumn/) { get; } | Índice mínimo de columna de esas celdas que han sido instanciadas en la colección (no incluye la columna donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda en ella). |
| [MinDataColumn](../../aspose.cells.gridweb.data/gridcells/mindatacolumn/) { get; } | Índice mínimo de columna de la celda que contiene datos. |
| [MinDataRow](../../aspose.cells.gridweb.data/gridcells/mindatarow/) { get; } | Índice de fila mínimo de la celda que contiene datos. |
| [MinRow](../../aspose.cells.gridweb.data/gridcells/minrow/) { get; } | Índice de fila mínimo de la celda que contiene datos o estilo. |
| [RowEnumerator](../../aspose.cells.gridweb.data/gridcells/rowenumerator/) { get; } | Obtiene el enumerador de filas |
| [Rows](../../aspose.cells.gridweb.data/gridcells/rows/) { get; } | Obtiene la colección de objetos [`GridRow`](../gridrow/) que representan las filas individuales en esta hoja de cálculo. |
| [StandardHeight](../../aspose.cells.gridweb.data/gridcells/standardheight/) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de puntos. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridcells/standardheightpixels/) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de píxeles. |
| [StandardWidth](../../aspose.cells.gridweb.data/gridcells/standardwidth/) { get; set; } | Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de caracteres. |
| [StandardWidthInch](../../aspose.cells.gridweb.data/gridcells/standardwidthinch/) { get; set; } | Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de pulgadas. |
| [StandardWidthPixels](../../aspose.cells.gridweb.data/gridcells/standardwidthpixels/) { get; set; } | Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de píxeles. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CheckCell](../../aspose.cells.gridweb.data/gridcells/checkcell/)(int, int) | Obtiene el elemento [`GridCell`](../gridcell/) o null en el índice de fila y columna de celda especificados. |
| [CheckColumn](../../aspose.cells.gridweb.data/gridcells/checkcolumn/)(int) | Obtiene el elemento [`GridColumn`](../gridcolumn/) o null en el índice de columna especificado. |
| [CheckRow](../../aspose.cells.gridweb.data/gridcells/checkrow/)(int) | Obtiene el elemento [`GridRow`](../gridrow/) o null en el índice de fila de celda especificado. |
| [Clear](../../aspose.cells.gridweb.data/gridcells/clear/)() | Borra todas las celdas de la colección. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | Borra el contenido de un rango. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | Borra el contenido de un rango. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats)(GridCellArea) | Borra el formato de un rango. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | Borra el formato de un rango. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange)(GridCellArea) | Borra el contenido y el formato de un rango. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | Borra el contenido y el formato de un rango. |
| [CopyColumn](../../aspose.cells.gridweb.data/gridcells/copycolumn/)(GridCells, int, int) | Copia los datos y formatos de una columna completa. |
| [CopyColumns](../../aspose.cells.gridweb.data/gridcells/copycolumns/)(GridCells, int, int, int) | Copia los datos y formatos de una columna completa. |
| [CopyRow](../../aspose.cells.gridweb.data/gridcells/copyrow/)(GridCells, int, int) | Copia los datos y formatos de una fila completa. |
| [CopyRows](../../aspose.cells.gridweb.data/gridcells/copyrows/)(GridCells, int, int, int) | Copia los datos y formatos de varias filas completas. |
| [DeleteBlankColumns](../../aspose.cells.gridweb.data/gridcells/deleteblankcolumns/)() | Elimina todas las columnas en blanco que no contengan ningún dato. |
| [DeleteBlankRows](../../aspose.cells.gridweb.data/gridcells/deleteblankrows/)() | Elimina todas las filas en blanco que no contienen datos. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn)(int) | Elimina una columna. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | Elimina una columna. |
| [DeleteColumns](../../aspose.cells.gridweb.data/gridcells/deletecolumns/)(int, int, bool) | Elimina varias columnas. |
| [DeleteRange](../../aspose.cells.gridweb.data/gridcells/deleterange/)(int, int, int, int, GridShiftType) | Elimina un rango de celdas y desplaza las celdas según la opción de desplazamiento. |
| [DeleteRow](../../aspose.cells.gridweb.data/gridcells/deleterow/)(int) | Elimina una fila. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows)(int, int) | Elimina varias filas. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | Elimina varias filas en la hoja de cálculo. |
| [Export](../../aspose.cells.gridweb.data/gridcells/export/)(int, int, int, int, bool, bool) | Exporta datos de la colección Cells de un WebWorksheet a un nuevo objeto DataTable |
| [ExportArray](../../aspose.cells.gridweb.data/gridcells/exportarray/)(int, int, int, int) | Exporta datos de la colección `GridCells` a un objeto matriz bidimensional. |
| [GetCell](../../aspose.cells.gridweb.data/gridcells/getcell/)(int, int) | Obtiene el elemento [`GridCell`](../gridcell/) en el índice de fila de celda y columna especificados. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/gridcells/getcolumnwidth/)(int) | Obtiene el ancho de la columna especificada |
| [GetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthinch/)(int) | Obtiene el ancho de la columna especificada, en unidades de pulgadas. |
| [GetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthpixel/)(int) | Obtiene el ancho de la columna especificada, en unidades de píxeles. |
| [GetEnumerator](../../aspose.cells.gridweb.data/gridcells/getenumerator/)() | Obtiene el enumerador de filas |
| [GetRow](../../aspose.cells.gridweb.data/gridcells/getrow/)(int) | Obtiene el elemento [`GridRow`](../gridrow/) en el índice de fila de celda especificado. |
| [GetRowHeight](../../aspose.cells.gridweb.data/gridcells/getrowheight/)(int) | Obtiene la altura de una fila especificada. |
| [GetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/getrowheightinch/)(int) | Obtiene la altura de una fila especificada en unidades de pulgadas. |
| [GetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/getrowheightpixel/)(int) | Obtiene la altura de una fila especificada en unidades de píxel. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/getrowoutlinelevel/)(int) | Obtiene el nivel de esquema de la fila. |
| [GetViewColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getviewcolumnwidthpixel/)(int) | Obtiene el ancho en diferentes tipos de vista. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns)(int, int) | Agrupa columnas. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | Agrupa columnas. |
| [GroupRows](../../aspose.cells.gridweb.data/gridcells/grouprows/)(int, int) | Agrupa filas. |
| [HideColumn](../../aspose.cells.gridweb.data/gridcells/hidecolumn/)(int) | Oculta una columna. |
| [HideRow](../../aspose.cells.gridweb.data/gridcells/hiderow/)(int) | Oculta una fila. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn)(int) | Inserta una nueva columna en la hoja de cálculo. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | Inserta una nueva columna en la hoja de cálculo. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns)(int, int) | Inserta algunas columnas en la hoja de cálculo. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | Inserta algunas columnas en la hoja de cálculo. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange)(GridCellArea, GridShiftType) | Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange_1)(GridCellArea, int, GridShiftType, bool) | Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento. |
| [InsertRow](../../aspose.cells.gridweb.data/gridcells/insertrow/)(int) | Inserta una nueva fila en la hoja de cálculo. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows)(int, int) | Inserta varias filas en la hoja de cálculo. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | Inserta varias filas en la hoja de cálculo. |
| [IsBlankColumn](../../aspose.cells.gridweb.data/gridcells/isblankcolumn/)(int) | Comprueba si la columna dada está vacía (no contiene datos). |
| [IsColumnHidden](../../aspose.cells.gridweb.data/gridcells/iscolumnhidden/)(int) | Comprueba si una columna en el índice dado está oculta. |
| [IsRowHidden](../../aspose.cells.gridweb.data/gridcells/isrowhidden/)(int) | Comprueba si una fila en el índice dado está oculta. |
| [Merge](../../aspose.cells.gridweb.data/gridcells/merge/)(int, int, int, int) | Fusiona un rango especificado de celdas en una sola celda. |
| [MoveRange](../../aspose.cells.gridweb.data/gridcells/moverange/)(GridCellArea, int, int) | Mueve el rango. |
| [RemoveDuplicates](../../aspose.cells.gridweb.data/gridcells/removeduplicates/)(int, int, int, int) | Elimina valores duplicados en el rango. |
| [RemoveFormulas](../../aspose.cells.gridweb.data/gridcells/removeformulas/)() | Elimina todas las fórmulas y las reemplaza con el valor de la fórmula. |
| [SetBorders](../../aspose.cells.gridweb.data/gridcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Establece bordes para un rango de celdas. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/gridcells/setcolumnwidth/)(int, double) | Establece el ancho de la columna especificada. |
| [SetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthinch/)(int, double) | Establece el ancho de la columna en unidades de pulgadas. |
| [SetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthpixel/)(int, int) | Establece el ancho de la columna en unidades de píxeles. |
| [SetRowHeight](../../aspose.cells.gridweb.data/gridcells/setrowheight/)(int, double) | Establece la altura de la fila especificada. |
| [SetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/setrowheightinch/)(int, double) | Establece la altura de la fila en unidades de pulgadas. |
| [SetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/setrowheightpixel/)(int, int) | Establece la altura de la fila en unidades de píxeles. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/setrowoutlinelevel/)(int, int) | Establece el nivel de esquema de la fila. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle_1)(string, GridTableItemStyle) | Establece el estilo a un rango especificado de celdas. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle)(int, int, int, int, GridTableItemStyle) | Establece el estilo a un rango especificado de celdas. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | Ordena los datos ascendente/descendente de arriba a abajo en un rango de una hoja de cálculo por el índice de columna especificado. Ordena los datos ascendente/descendente de izquierda a derecha en un rango de una hoja de cálculo por el índice de fila especificado. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | Ordena los datos ascendente/descendente de arriba a abajo en un rango de una hoja de cálculo por el índice de columna especificado. Ordena los datos ascendente/descendente de izquierda a derecha en un rango de una hoja de cálculo por el índice de fila especificado. |
| [UngroupColumns](../../aspose.cells.gridweb.data/gridcells/ungroupcolumns/)(int, int) | Desagrupa columnas. |
| [UngroupRows](../../aspose.cells.gridweb.data/gridcells/ungrouprows/)(int, int) | Desagrupa filas. |
| [UnhideColumn](../../aspose.cells.gridweb.data/gridcells/unhidecolumn/)(int, double) | Muestra una columna |
| [UnhideRow](../../aspose.cells.gridweb.data/gridcells/unhiderow/)(int) | Muestra una fila. |
| [UnMerge](../../aspose.cells.gridweb.data/gridcells/unmerge/)(int, int, int, int) | Descombina un rango especificado de celdas combinadas. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/gridcells/cellindextoname/)(int, int) | Obtiene el nombre de la celda según sus índices de fila y columna. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/gridcells/cellnametoindex/)(string, out int, out int) | Obtiene los índices de fila y columna de la celda según su nombre |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/gridcells/columnindextoname/)(int) | Obtiene el nombre de la columna según el índice de columna. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/gridcells/columnnametoindex/)(string) | Obtiene el índice de columna según el nombre de columna. |

### Ver también

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


