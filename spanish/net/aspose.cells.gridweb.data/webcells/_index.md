---
title: "Clase WebCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.Data.WebCells."
type: docs
url: /es/net/aspose.cells.gridweb.data/webcells/
---
## WebCells class

```csharp
[Obsolete("This class is obsolete; use  GridCells instead")]
public class WebCells
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/webcells/count/) { get; } | Obtiene el número de celdas. |
| [Item](../../aspose.cells.gridweb.data/webcells/item/) { get; } | Obtiene el elemento Cell en el índice de fila y columna de celda especificados. (2 indexadores) |
| [MaxColumn](../../aspose.cells.gridweb.data/webcells/maxcolumn/) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/webcells/maxrow/) { get; } |  |
| [MergedCells](../../aspose.cells.gridweb.data/webcells/mergedcells/) { get; } | Obtiene la colección de celdas combinadas. |
| [MinColumn](../../aspose.cells.gridweb.data/webcells/mincolumn/) { get; } | Número mínimo de columna de la celda que contiene datos o estilo. |
| [MinRow](../../aspose.cells.gridweb.data/webcells/minrow/) { get; } | Número mínimo de fila de la celda que contiene datos o estilo. |
| [StandardHeight](../../aspose.cells.gridweb.data/webcells/standardheight/) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de puntos. |
| [StandardWidth](../../aspose.cells.gridweb.data/webcells/standardwidth/) { get; set; } | Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de caracteres. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/webcells/clear/)() |  |
| [ClearContents](../../aspose.cells.gridweb.data/webcells/clearcontents/)(int, int, int, int) | Borra el contenido de un rango. |
| [DeleteColumn](../../aspose.cells.gridweb.data/webcells/deletecolumn/)(int) | Elimina una columna. |
| [DeleteRow](../../aspose.cells.gridweb.data/webcells/deleterow/)(int) | Elimina una fila. |
| [DeleteRows](../../aspose.cells.gridweb.data/webcells/deleterows/)(int, int) | Elimina un número de filas. Este método es mucho más rápido que DeleteRow al realizar una eliminación de filas por lotes. |
| [Export](../../aspose.cells.gridweb.data/webcells/export/)(int, int, int, int, bool, bool) | Exporta datos de la colección Cells de un WebWorksheet a un nuevo objeto DataTable |
| [ExportArray](../../aspose.cells.gridweb.data/webcells/exportarray/)(int, int, int, int) | Exporta datos de la colección Cells a un objeto de matriz bidimensional. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/webcells/getcolumncaption/)(int) | Obtiene el título de la columna. Si el título no está establecido, devuelve una cadena vacía. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/webcells/getcolumnreadonly/)(int) | Obtiene si una columna es de solo lectura. Este es un método extendido de GridWeb específicamente, no se conservará ni tendrá efecto en el archivo Excel real. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/webcells/getcolumnwidth/)(int) | Obtiene el ancho de la columna especificada |
| [GetEnumerator](../../aspose.cells.gridweb.data/webcells/getenumerator/)() | Obtiene el enumerador de celdas |
| [GetRowCaption](../../aspose.cells.gridweb.data/webcells/getrowcaption/)(int) | Obtiene el título de la fila. Si el título no está establecido, devuelve una cadena vacía. |
| [GetRowHeight](../../aspose.cells.gridweb.data/webcells/getrowheight/)(int) | Obtiene la altura de una fila especificada. |
| [GetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/getrowhiddenstatus/)(int) | Obtiene el estado oculto de una fila especificada. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/getrowoutlinelevel/)(int) | Obtiene el nivel de esquema de la fila. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/webcells/getrowreadonly/)(int) | Obtiene si una fila es de solo lectura. este es un método extendido de GridWeb específicamente, no se conservará ni tendrá efecto en el archivo Excel real |
| [InsertColumn](../../aspose.cells.gridweb.data/webcells/insertcolumn/)(int) | Inserta una nueva columna en la hoja de cálculo. |
| [InsertRow](../../aspose.cells.gridweb.data/webcells/insertrow/)(int) | Inserta una nueva fila en la hoja de cálculo. |
| [InsertRows](../../aspose.cells.gridweb.data/webcells/insertrows/)(int, int) | Inserta varias filas en la hoja de cálculo. |
| [Merge](../../aspose.cells.gridweb.data/webcells/merge/)(int, int, int, int) |  |
| [SetBorders](../../aspose.cells.gridweb.data/webcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Establece bordes para un rango de celdas. |
| [SetColumnCaption](../../aspose.cells.gridweb.data/webcells/setcolumncaption/)(int, string) | Establece el título para la columna.por favor, tenga en cuenta que este es un atributo de extensión y no se conserva en el archivo Excel |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/webcells/setcolumnreadonly/)(int, bool) | Establece una columna como de solo lectura para que el usuario no pueda eliminarla desde el lado del cliente. este es un método extendido de GridWeb específicamente, no se conservará ni tendrá efecto en el archivo Excel real |
| [SetColumnWidth](../../aspose.cells.gridweb.data/webcells/setcolumnwidth/)(int, Unit) | Establece el ancho de la columna especificada. El tipo de ancho aceptado es Point, Pixel o Inch. |
| [SetRowCaption](../../aspose.cells.gridweb.data/webcells/setrowcaption/)(int, string) | Establece el título para la fila. |
| [SetRowHeight](../../aspose.cells.gridweb.data/webcells/setrowheight/)(int, Unit) | Establece la altura de la fila especificada. El tipo de ancho aceptado es Point, Pixel o Inch. |
| [SetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/setrowhiddenstatus/)(int, bool) | Establece el estado oculto de una fila especificada. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevel/)(int, int) | Establece el nivel de esquema de la fila. |
| [SetRowOutlineLevelAndStatus](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevelandstatus/)(int, int, bool) | Establece el nivel de esquema de la fila. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/webcells/setrowreadonly/)(int, bool) | Establece una fila como de solo lectura para que el usuario no pueda eliminarla desde el lado del cliente. este es un método extendido de GridWeb específicamente, no se conservará ni tendrá efecto en el archivo Excel real |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle_1)(string, TableItemStyle) | Establece el estilo a un rango especificado de celdas. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle)(int, int, int, int, TableItemStyle) | Establece el estilo a un rango especificado de celdas. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort)(int, int, int, int, int) | Ordena los datos de forma ascendente de arriba a abajo en un rango de un WebWorksheet por el índice de columna especificado. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_2)(int, int, int, int, int[]) | Ordena los datos de forma ascendente de arriba a abajo en un rango de un WebWorksheet por algunos campos especificados mediante una matriz de índices de columnas. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_1)(int, int, int, int, int, SortByOrder, SortOrientation, bool) | Ordena los datos de forma ascendente de arriba a abajo en un rango de un WebWorksheet por el índice de columna especificado. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_3)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | Ordena los datos de forma ascendente en un rango de un WebWorksheet por algunos campos especificados mediante una matriz de índices. |
| [UnMerge](../../aspose.cells.gridweb.data/webcells/unmerge/)(int, int, int, int) | Descombina un rango especificado de celdas combinadas. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/webcells/cellindextoname/)(int, int) | Obtiene el nombre de la celda según sus índices de fila y columna. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/webcells/cellnametoindex/)(string, out int, out int) | Obtiene los índices de fila y columna de la celda según su nombre |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/webcells/columnindextoname/)(int) | Obtiene el nombre de la columna según el índice de columna. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/webcells/columnnametoindex/)(string) | Obtiene el índice de columna según el nombre de columna. |

### Observaciones

NOTA: Esta clase está ahora obsoleta. Por favor, use GridCells en su lugar. Esta clase será eliminada después de 6 meses desde agosto de 2014. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ver también

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


