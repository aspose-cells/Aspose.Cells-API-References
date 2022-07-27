---
title: Cells
second_title: Referencia de API de Aspose.Cells para .NET
description: Encapsula una colección de objetos relevantes para la celda comoCell./cell Row./row ...etc.
type: docs
weight: 300
url: /es/net/aspose.cells/cells/
---
## Cells class

Encapsula una colección de objetos relevantes para la celda, como[`Cell`](../cell) ,[`Row`](../row) ...etc.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns) { get; } | Obtiene la colección de[`Column`](../column) objetos que representan las columnas individuales en esta hoja de trabajo. |
| [Count](../../aspose.cells/cells/count) { get; } | Obtiene el recuento total de objetos Cell instanciados. |
| [CountLarge](../../aspose.cells/cells/countlarge) { get; } | Obtiene el recuento total de objetos Cell instanciados. |
| [FirstCell](../../aspose.cells/cells/firstcell) { get; } | Obtiene la primera celda de esta hoja de cálculo. |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched) { get; set; } | Indica que la altura de fila y la altura de fuente predeterminada coinciden con |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden) { get; set; } | Indica si la fila está oculta por defecto. |
| [Item](../../aspose.cells/cells/item) { get; } | Obtiene el[`Cell`](../cell) elemento en el índice de fila de celda y el índice de columna especificados. (2 indexers) |
| [LastCell](../../aspose.cells/cells/lastcell) { get; } | Obtiene la última celda de esta hoja de cálculo. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn) { get; } | Índice de columna mínimo de aquellas celdas que se han instanciado en la colección (no incluye la columna donde se define el estilo para toda la columna pero no se ha instanciado ninguna celda). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn) { get; } | Índice de columna máximo de celda que contiene datos. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow) { get; } | Índice de fila máximo de celda que contiene datos. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange) { get; } | Obtiene el rango máximo que incluye datos, celdas combinadas y formas. |
| [MaxRow](../../aspose.cells/cells/maxrow) { get; } | Índice de fila máximo de celda que contiene datos o estilo. |
| [MemorySetting](../../aspose.cells/cells/memorysetting) { get; set; } | Obtiene o establece la opción de uso de memoria para estas celdas. |
| [MergedCells](../../aspose.cells/cells/mergedcells) { get; } | Obtiene la colección de celdas combinadas. |
| [MinColumn](../../aspose.cells/cells/mincolumn) { get; } | Índice de columna mínimo de aquellas celdas que se han instanciado en la colección (no incluye la columna donde se define el estilo para toda la columna pero no se ha instanciado ninguna celda). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn) { get; } | Índice de columna mínimo de celda que contiene datos. |
| [MinDataRow](../../aspose.cells/cells/mindatarow) { get; } | Índice de fila mínimo de celda que contiene datos. |
| [MinRow](../../aspose.cells/cells/minrow) { get; } | Índice de fila mínimo de celda que contiene datos o estilo. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading) { get; set; } | Obtiene o establece si el modelo de datos de celdas debe admitir la lectura de subprocesos múltiples. El valor predeterminado de esta propiedad es falso. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields) { get; } | Obtiene la lista de campos de ods. |
| [PreserveString](../../aspose.cells/cells/preservestring) { get; set; } | Obtiene o establece un valor que indica si todos los valores de la hoja de cálculo se conservan como cadenas. El valor predeterminado es falso. |
| [Ranges](../../aspose.cells/cells/ranges) { get; } | Obtiene la colección de[`Range`](../range)objetos creados en tiempo de ejecución. |
| [Rows](../../aspose.cells/cells/rows) { get; } | Obtiene la colección de[`Row`](../row) objetos que representan las filas individuales en esta hoja de trabajo. |
| [StandardHeight](../../aspose.cells/cells/standardheight) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de puntos. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de pulgadas. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels) { get; set; } | Obtiene o establece el alto de fila predeterminado en esta hoja de cálculo, en unidades de píxeles. |
| [StandardWidth](../../aspose.cells/cells/standardwidth) { get; set; } | Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de caracteres. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch) { get; set; } | Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de pulgadas. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels) { get; set; } | Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de píxeles. |
| [Style](../../aspose.cells/cells/style) { get; set; } | Obtiene y establece el estilo predeterminado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange)(Range) | Agrega una referencia de objeto de rango a las celdas |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle)(int, Style, StyleFlag) | Aplica formatos para una columna completa. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle)(int, Style, StyleFlag) | Aplica formatos para una fila completa. |
| [ApplyStyle](../../aspose.cells/cells/applystyle)(Style, StyleFlag) | Aplica formatos para una hoja de cálculo completa. |
| [CheckCell](../../aspose.cells/cells/checkcell)(int, int) | Obtiene el[`Cell`](../cell) elemento o nulo en el índice de fila de celda y el índice de columna especificados. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn)(int) | Obtiene el[`Column`](../column) elemento o nulo en la columna especificada index. |
| [CheckRow](../../aspose.cells/cells/checkrow)(int) | Obtiene el[`Row`](../row) elemento o en la fila de celda especificada index. |
| [Clear](../../aspose.cells/cells/clear)() | Borra todos los objetos de fila y celda. |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents)(CellArea) | Borra el contenido de un rango. |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents_1)(int, int, int, int) | Borra el contenido de un rango. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats)(CellArea) | Borra el formato de un rango. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats_1)(int, int, int, int) | Borra el formato de un rango. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells)() | Borra todos los rangos combinados. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange)(CellArea) | Borra el contenido y el formato de un rango. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange_1)(int, int, int, int) | Borra el contenido y el formato de un rango. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue)() | Convierte datos de cadena en celdas a valor numérico si es posible. |
| [CopyColumn](../../aspose.cells/cells/copycolumn)(Cells, int, int) | Copia datos y formatos de una columna completa. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns)(Cells, int, int, int) | Copia datos y formatos de una columna completa. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_2)(Cells, int, int, int, int) | Copia datos y formatos de todas las columnas. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_1)(Cells, int, int, int, PasteOptions) | Copia datos y formatos de una columna completa. |
| [CopyRow](../../aspose.cells/cells/copyrow)(Cells, int, int) | Copia datos y formatos de una fila completa. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows)(Cells, int, int, int) | Copia datos y formatos de algunas filas completas. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_1)(Cells, int, int, int, CopyOptions) | Copia datos y formatos de algunas filas completas. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | Copia datos y formatos de algunas filas completas. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_2)(string) | Crea un[`Range`](../range) objeto de una dirección del rango. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_3)(string, string) | Crea un[`Range`](../range) objeto de un rango de celdas. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange)(int, int, bool) | Crea un[`Range`](../range) objeto de filas de celdas o columnas de celdas. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_1)(int, int, int, int) | Crea un[`Range`](../range) objeto de un rango de celdas. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns)() | Eliminar todas las columnas en blanco que no contengan ningún dato. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns_1)(DeleteOptions) | Eliminar todas las columnas en blanco que no contengan ningún dato. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows)() | Eliminar todas las filas en blanco que no contienen ningún dato. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows_1)(DeleteOptions) | Eliminar todas las filas en blanco que no contienen ningún dato. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn)(int) | Elimina una columna. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn_1)(int, bool) | Elimina una columna. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns)(int, int, bool) | Elimina varias columnas. |
| [DeleteRange](../../aspose.cells/cells/deleterange)(int, int, int, int, ShiftType) | Elimina un rango de celdas y desplaza celdas según la opción de desplazamiento. |
| [DeleteRow](../../aspose.cells/cells/deleterow)(int) | Elimina una fila. |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows)(int, int) | Elimina varias filas. |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows_1)(int, int, bool) | Elimina varias filas en la hoja de cálculo. |
| [Dispose](../../aspose.cells/cells/dispose)() | Realiza tareas definidas por la aplicación asociadas con la liberación, liberación o restablecimiento de recursos no administrados. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn)(short) | Obtiene la última celda de esta columna. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn_1)(int, int, short, short) | Obtiene la última celda con índice de columna máximo en este rango. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow)(int) | Obtiene la última celda de esta fila. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow_1)(int, int, int, int) | Obtiene la última celda con índice de fila máximo en este rango. |
| [ExportArray](../../aspose.cells/cells/exportarray)(int, int, int, int) | Exporta datos en el[`Cells`](../cells) colección a un objeto de matriz de dos dimensiones. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable)(int, int, int, int) | Exporta datos en el[`Cells`](../cells) colección a unDataTable objeto. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_2)(int, int, int, int, bool) | Exporta datos en el[`Cells`](../cells) colección a unDataTable objeto. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_1)(int, int, int, int, ExportTableOptions) | Exporta datos en el[`Cells`](../cells) colección a unDataTable objeto. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring)(int, int, int, int) | Exporta datos en el[`Cells`](../cells) colección a unDataTable objeto. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring_1)(int, int, int, int, bool) | Exporta datos en el[`Cells`](../cells) colección a unDataTable objeto. |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray)(int, int, int, int) | Exporta el tipo de valor de celda en el[`Cells`](../cells) colección a un objeto de matriz de dos dimensiones. |
| [Find](../../aspose.cells/cells/find#find)(object, Cell) | Encuentra la celda que contiene el objeto de entrada. |
| [Find](../../aspose.cells/cells/find#find_1)(object, Cell, FindOptions) | Encuentra la celda que contiene el objeto de entrada. |
| [GetCell](../../aspose.cells/cells/getcell)(int, int) | Obtiene el[`Cell`](../cell) elemento o nulo en el índice de fila de celda y el índice de columna especificados. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle)(int, int) | Obtiene el estilo de la celda dada. |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth)(int) | Obtiene el ancho de la columna especificada en vista normal |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch)(int) | Obtiene el ancho de la columna especificada en vista normal, en unidades de pulgadas. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel)(int) | Obtiene el ancho de la columna especificada en la vista normal, en unidades de píxel. |
| [GetDependents](../../aspose.cells/cells/getdependents)(bool, int, int) | Obtiene todas las celdas que hacen referencia a la celda específica. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation)(int, int, bool) | Obtiene todas las celdas cuyo resultado calculado depende de una celda específica. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator)() | Obtiene el enumerador de celdas. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel)(int) | Obtiene el nivel de esquema (basado en cero) de la columna. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel)(int) | Obtiene el nivel de esquema (basado en cero) de la fila. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow)(int) | Obtiene el índice de la última fila de la celda que contiene datos en la columna especificada. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel)() | Obtiene el nivel máximo de esquema de columna agrupada (basado en cero). |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel)() | Obtiene el nivel máximo de esquema de filas agrupadas (basado en cero). |
| [GetRow](../../aspose.cells/cells/getrow)(int) | Obtiene el[`Row`](../row) elemento en la fila de celda especificada index. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator)() | Obtiene el enumerador de filas. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight)(int) | Obtiene la altura de una fila especificada. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch)(int) | Obtiene la altura de una fila especificada en unidades de pulgadas. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel)(int) | Obtiene la altura de una fila especificada en unidades de píxel. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint)(int) | Obtiene la altura de la fila original en unidades de punto si la fila está oculta |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel)(int) | Obtener el ancho en diferente tipo de vista. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight)(int) | Obtiene la altura de una fila especificada. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch)(int) | Obtiene la altura de una fila especificada en unidades de pulgadas. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns)(int, int) | Agrupa columnas. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns_1)(int, int, bool) | Agrupa columnas. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows)(int, int) | Agrupa filas. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows_1)(int, int, bool) | Agrupa filas. |
| [HideColumn](../../aspose.cells/cells/hidecolumn)(int) | Oculta una columna. |
| [HideColumns](../../aspose.cells/cells/hidecolumns)(int, int) | Ocultar varias columnas. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail)(bool, int) | Contrae las filas/columnas agrupadas. |
| [HideRow](../../aspose.cells/cells/hiderow)(int) | Oculta una fila. |
| [HideRows](../../aspose.cells/cells/hiderows)(int, int) | Oculta varias filas. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_1)(double[], int, int, bool) | Importa una matriz de double en una hoja de trabajo. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_3)(int[], int, int, bool) | Importa una matriz de enteros a una hoja de cálculo. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_5)(string[], int, int, bool) | Importa una matriz de cadenas en una hoja de trabajo. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist)(ArrayList, int, int, bool) | Importa una lista de matriz de datos en una hoja de trabajo. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv)(Stream, TxtLoadOptions, int, int) | Importa un archivo CSV a las celdas. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_2)(string, TxtLoadOptions, int, int) | Importa un archivo CSV a las celdas. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_1)(Stream, string, bool, int, int) | Importa un archivo CSV a las celdas. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_3)(string, string, bool, int, int) | Importa un archivo CSV a las celdas. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects)(ICollection, int, int, ImportTableOptions) | Importa objetos personalizados. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | Importa objetos personalizados. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_3)(IDataReader, int, int) | Importa datos de unIDataReader objeto. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_1)(DataTable, int, int, ImportTableOptions) | Importar datos de la tabla de datos personalizados. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_2)(DataView, int, int, ImportTableOptions) | Importar datos desde la vista de datos. |
| [ImportData](../../aspose.cells/cells/importdata#importdata)(ICellsDataTable, int, int, ImportTableOptions) | Importar datos de la tabla de datos personalizados. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_4)(IDataReader, int, int, ImportTableOptions) | Importa datos de unIDataReader objeto. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid)(DataGrid, int, int, bool) | Importa unDataGrid en una hoja de trabajo. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_1)(DataGrid, int, int, int, int, bool) | Importa unDataGrid en una hoja de trabajo. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | Importa unDataGrid en una hoja de trabajo. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring)(DataGrid, int, int, bool) | Importa unDataGrid en una hoja de trabajo. Este método no intenta convertir texto en valores numéricos. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow)(DataRow, int, int) | Importa un DataRow al archivo de Excel. |
| [ImportDataView](../../aspose.cells/cells/importdataview#importdataview_3)(DataView, int, int) | Importa unDataView en una hoja de trabajo. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray)(string[], int, int, bool) | Importa una matriz de fórmulas en una hoja de trabajo. |
| [ImportGridView](../../aspose.cells/cells/importgridview)(GridView, int, int, ImportTableOptions) | Importa una vista de cuadrícula a estas celdas. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray)(object[], int, int, bool) | Importa una matriz de datos en una hoja de trabajo. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray_1)(object[], int, int, bool, int) | Importa una matriz de datos en una hoja de trabajo. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn)(int) | Inserta una nueva columna en la hoja de cálculo. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn_1)(int, bool) | Inserta una nueva columna en la hoja de cálculo. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns)(int, int) | Inserta algunas columnas en la hoja de trabajo. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns_1)(int, int, bool) | Inserta algunas columnas en la hoja de trabajo. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells)(Range, int, int, ShiftType) | Insertar rango de corte. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange)(CellArea, ShiftType) | Inserta un rango de celdas y desplaza celdas según la opción de desplazamiento. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_1)(CellArea, int, ShiftType) | Inserta un rango de celdas y desplaza celdas según la opción de desplazamiento. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_2)(CellArea, int, ShiftType, bool) | Inserta un rango de celdas y desplaza celdas según la opción de desplazamiento. |
| [InsertRow](../../aspose.cells/cells/insertrow)(int) | Inserta una nueva fila en la hoja de cálculo. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows)(int, int) | Inserta varias filas en la hoja de trabajo. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_2)(int, int, bool) | Inserta varias filas en la hoja de trabajo. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_1)(int, int, InsertOptions) | Inserta varias filas en la hoja de trabajo. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn)(int) | Comprueba si la columna dada está en blanco (no contiene ningún dato). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden)(int) | Comprueba si una columna en el índice dado está oculta. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled)(int, int, int, int) | Comprobar si se pudo eliminar el rango. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden)(int) | Comprueba si una fila en el índice dado está oculta. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap)(string, int, int, string) | Enlace a un mapa xml. |
| [Merge](../../aspose.cells/cells/merge#merge)(int, int, int, int) | Combina un rango específico de celdas en una sola celda. |
| [Merge](../../aspose.cells/cells/merge#merge_1)(int, int, int, int, bool) | Combina un rango específico de celdas en una sola celda. |
| [Merge](../../aspose.cells/cells/merge#merge_2)(int, int, int, int, bool, bool) | Combina un rango específico de celdas en una sola celda. |
| [MoveRange](../../aspose.cells/cells/moverange)(CellArea, int, int) | Mueve el rango. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates)() | Elimina filas duplicadas en la hoja. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_1)(int, int, int, int) | Elimina valores duplicados en el rango. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_2)(int, int, int, int, bool, int[]) | Elimina datos duplicados del rango. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas)() | Elimina todas las fórmulas y las reemplaza con el valor de la fórmula. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting)(CellArea) | Recupera la configuración de subtotales del rango. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth)(int, double) | Establece el ancho de la columna especificada en vista normal. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch)(int, double) | Establece el ancho de columna en unidades de pulgadas en la vista normal. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel)(int, int) | Establece el ancho de columna en unidades de píxeles en la vista normal. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight)(int, double) | Establece la altura de la fila especificada. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch)(int, double) | Establece la altura de fila en unidades de pulgadas. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel)(int, int) | Establece la altura de la fila en unidades de píxeles. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel)(int, int) | Establece el ancho de la columna en una vista diferente. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail)(bool, int) | Expande las filas/columnas agrupadas. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal)(CellArea, int, ConsolidationFunction, int[]) | Crea subtotales para el rango. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Crea subtotales para el rango. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns)(int, int, int, TxtLoadOptions) | Divide el texto de la columna en columnas. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns)(int, int) | Desagrupa columnas. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows)(int, int) | Desagrupa filas. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows_1)(int, int, bool) | Desagrupa filas. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn)(int, double) | Muestra una columna |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns)(int, int, double) | Mostrar múltiples columnas. |
| [UnhideRow](../../aspose.cells/cells/unhiderow)(int, double) | Muestra una fila. |
| [UnhideRows](../../aspose.cells/cells/unhiderows)(int, int, double) | Muestra las filas ocultas. |
| [UnMerge](../../aspose.cells/cells/unmerge)(int, int, int, int) | Separa un rango específico de celdas combinadas. |

### Ejemplos

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Establecer altura de fila predeterminada
cells.StandardHeight = 20;
//Establecer altura de fila
cells.SetRowHeight(2, 20.5);

// Establecer el ancho de columna predeterminado
cells.StandardWidth = 15;
//Establecer ancho de columna
cells.SetColumnWidth(3, 12.57);

//Combinar células
cells.Merge(5, 4, 2, 2);

// Poner valores a las celdas
cells[0, 0].PutValue(true);
cells[0, 1].PutValue(1);
cells[0, 2].PutValue("abc");

//Exportar datos
object[,] arr = cells.ExportArray(0, 0, 10, 10);

[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells

'Establecer altura de fila predeterminada
cells.StandardHeight = 20
'Establecer altura de fila
cells.SetRowHeight(2, 20.5)

'Establecer el ancho de columna predeterminado
cells.StandardWidth = 15
'Establecer ancho de columna
cells.SetColumnWidth(3, 12.57)

'Combinar células
cells.Merge(5, 4, 2, 2)

'Exportar datos
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### Ver también

* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
