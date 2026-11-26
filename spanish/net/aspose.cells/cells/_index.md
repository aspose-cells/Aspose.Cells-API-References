---
title: "Clase Cells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Cells class. Encapsula una colección de objetos relevantes de celda como Cell Row ...etc"
type: docs
url: /es/net/aspose.cells/cells/
---
## Cells class

Encapsula una colección de objetos relevantes de celda, como [`Cell`](../cell/), [`Row`](../row/), ...etc.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns/) { get; } | Obtiene la colección de objetos [`Column`](../column/) que representan las columnas individuales en esta hoja de cálculo. |
| [Count](../../aspose.cells/cells/count/) { get; } | Obtiene el recuento total de objetos Cell instanciados. |
| [CountLarge](../../aspose.cells/cells/countlarge/) { get; } | Obtiene el recuento total de objetos Cell instanciados. |
| [FirstCell](../../aspose.cells/cells/firstcell/) { get; } | Obtiene la primera celda en esta hoja de cálculo. |
| [IsDefaultColumnHidden](../../aspose.cells/cells/isdefaultcolumnhidden/) { get; set; } |  |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched/) { get; set; } | Indica que la altura de la fila y la altura de fuente predeterminada coinciden. |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden/) { get; set; } | Indica si la fila está oculta por defecto. |
| [Item](../../aspose.cells/cells/item/) { get; } | Obtiene el elemento [`Cell`](../cell/) en el índice de fila y columna de celda especificados. (2 indexadores) |
| [LastCell](../../aspose.cells/cells/lastcell/) { get; } | Obtiene la última celda en esta hoja de cálculo. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn/) { get; } | Índice máximo de columna de esas celdas que han sido instanciadas en la colección (no incluye la columna donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda en ella). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn/) { get; } | Índice máximo de columna de la celda que contiene datos. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow/) { get; } | Índice máximo de fila de la celda que contiene datos. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange/) { get; } | Obtiene el rango máximo que incluye datos, celdas combinadas y formas. |
| [MaxRow](../../aspose.cells/cells/maxrow/) { get; } | Índice máximo de fila de la celda que contiene datos o estilo. |
| [MemorySetting](../../aspose.cells/cells/memorysetting/) { get; set; } | Obtiene o establece la opción de uso de memoria para estas celdas. |
| [MergedCells](../../aspose.cells/cells/mergedcells/) { get; } | (**Obsolete.**) Obtiene la colección de celdas combinadas. |
| [MinColumn](../../aspose.cells/cells/mincolumn/) { get; } | Índice mínimo de columna de esas celdas que han sido instanciadas en la colección (no incluye la columna donde el estilo está definido para toda la columna pero no se ha instanciado ninguna celda en ella). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn/) { get; } | Índice mínimo de columna de la celda que contiene datos. |
| [MinDataRow](../../aspose.cells/cells/mindatarow/) { get; } | Índice de fila mínimo de la celda que contiene datos. |
| [MinRow](../../aspose.cells/cells/minrow/) { get; } | Índice de fila mínimo de la celda que contiene datos o estilo. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading/) { get; set; } | Obtiene o establece si el modelo de datos de las celdas debe soportar lectura Multi-Thread. El valor predeterminado de esta propiedad es false. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields/) { get; } | Obtiene la lista de campos de ods. |
| [PreserveString](../../aspose.cells/cells/preservestring/) { get; set; } | Obtiene o establece un valor que indica si todos los valores de la hoja de cálculo se conservan como cadenas. El valor predeterminado es false. |
| [Ranges](../../aspose.cells/cells/ranges/) { get; } | Obtiene la colección de objetos [`Range`](../range/) creados en tiempo de ejecución. |
| [Rows](../../aspose.cells/cells/rows/) { get; } | Obtiene la colección de objetos [`Row`](../row/) que representan las filas individuales en esta hoja de cálculo. |
| [StandardHeight](../../aspose.cells/cells/standardheight/) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de puntos. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch/) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de pulgadas. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels/) { get; set; } | Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de píxeles. |
| [StandardWidth](../../aspose.cells/cells/standardwidth/) { get; set; } | Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de caracteres. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch/) { get; set; } | Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de pulgadas. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels/) { get; set; } | Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de píxeles. |
| [Style](../../aspose.cells/cells/style/) { get; set; } | Obtiene y establece el estilo predeterminado de la hoja de cálculo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange/)(Range) | Agrega una referencia de objeto de rango a las celdas |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle/)(int, Style, StyleFlag) | Aplica formatos a toda una columna. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle/)(int, Style, StyleFlag) | Aplica formatos a toda la fila. |
| [ApplyStyle](../../aspose.cells/cells/applystyle/)(Style, StyleFlag) | Aplica formatos a toda la hoja de cálculo. |
| [CheckCell](../../aspose.cells/cells/checkcell/)(int, int) | Obtiene el elemento [`Cell`](../cell/) o null en el índice de fila y columna de celda especificados. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn/)(int) | Obtiene el elemento [`Column`](../column/) o null en el índice de columna especificado. |
| [CheckRow](../../aspose.cells/cells/checkrow/)(int) | Obtiene el elemento [`Row`](../row/) o null en el índice de fila de celda especificado. |
| [Clear](../../aspose.cells/cells/clear/)() | Borra todos los datos de la hoja de cálculo. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents)(CellArea) | Borra el contenido de un rango. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents_1)(int, int, int, int) | Borra el contenido de un rango. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats)(CellArea) | Borra el formato de un rango. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats_1)(int, int, int, int) | Borra el formato de un rango. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells/)() | Borra todos los rangos combinados. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange)(CellArea) | Borra el contenido y el formato de un rango. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange_1)(int, int, int, int) | Borra el contenido y el formato de un rango. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue/)() | Convierte todos los datos de tipo cadena en la hoja de cálculo a valor numérico si es posible. |
| [CopyColumn](../../aspose.cells/cells/copycolumn/)(Cells, int, int) | Copia los datos y formatos de una columna completa. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns)(Cells, int, int, int) | Copia los datos y formatos de columnas completas. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_2)(Cells, int, int, int, int) | Copia los datos y formatos de todas las columnas. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_1)(Cells, int, int, int, PasteOptions) | Copia los datos y formatos de una columna completa. |
| [CopyRow](../../aspose.cells/cells/copyrow/)(Cells, int, int) | Copia los datos y formatos de una fila completa. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows)(Cells, int, int, int) | Copia los datos y formatos de algunas filas completas. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_1)(Cells, int, int, int, CopyOptions) | Copia los datos y formatos de algunas filas completas. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | Copia los datos y formatos de algunas filas completas. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_2)(string) | Crea un objeto [`Range`](../range/) a partir de una dirección del rango. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_3)(string, string) | Crea un objeto [`Range`](../range/) a partir de un rango de celdas. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange)(int, int, bool) | Crea un objeto [`Range`](../range/) a partir de filas de celdas o columnas de celdas. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_1)(int, int, int, int) | Crea un objeto [`Range`](../range/) a partir de un rango de celdas. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns)() | Elimina todas las columnas en blanco que no contengan ningún dato. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns_1)(DeleteOptions) | Elimina todas las columnas en blanco que no contengan ningún dato. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows)() | Elimina todas las filas en blanco que no contengan ningún dato u otro objeto. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows_1)(DeleteOptions) | Elimina todas las filas en blanco que no contengan ningún dato o algunos objetos especiales como comentarios visibles, tabla dinámica. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn)(int) | Elimina una columna. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn_1)(int, bool) | Elimina una columna. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns_1)(int, int, bool) | Elimina varias columnas. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns)(int, int, DeleteOptions) | Elimina varias columnas. |
| [DeleteRange](../../aspose.cells/cells/deleterange/)(int, int, int, int, ShiftType) | Elimina un rango de celdas y desplaza las celdas según la opción de desplazamiento. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow)(int) | Elimina una fila. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow_1)(int, bool) | Elimina una fila. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows)(int, int) | Elimina varias filas. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_2)(int, int, bool) | Elimina varias filas en la hoja de cálculo. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_1)(int, int, DeleteOptions) | Elimina varias filas en la hoja de cálculo. |
| [Dispose](../../aspose.cells/cells/dispose/)() | Ejecuta tareas definidas por la aplicación asociadas con liberar, liberar o restablecer recursos no administrados. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn)(int) | Obtiene la última celda en esta columna. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn_1)(int, int, int, int) | Obtiene la última celda con el índice de columna máximo en este rango. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow)(int) | Obtiene la última celda en esta fila. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow_1)(int, int, int, int) | Obtiene la última celda con el índice de fila máximo en este rango. |
| [ExportArray](../../aspose.cells/cells/exportarray/)(int, int, int, int) | Exporta los datos de la colección `Cells` a un objeto de matriz bidimensional. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable)(int, int, int, int) | Exporta los datos de la colección `Cells` a un objeto DataTable. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_2)(int, int, int, int, bool) | Exporta los datos de la colección `Cells` a un objeto DataTable. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_1)(int, int, int, int, ExportTableOptions) | Exporta los datos de la colección `Cells` a un objeto DataTable. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring)(int, int, int, int) | Exporta los datos de la colección `Cells` a un objeto DataTable. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring_1)(int, int, int, int, bool) | Exporta los datos de la colección `Cells` a un objeto DataTable. |
| [ExportList&lt;T&gt;](../../aspose.cells/cells/exportlist/)(int, int, int, int, ExportTableOptions) |  |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray/)(int, int, int, int) | Exporta el tipo de valor de celda en la colección `Cells` a un objeto de matriz bidimensional. |
| [Find](../../aspose.cells/cells/find/#find)(object, Cell) | Encuentra la celda que contiene el objeto de entrada. |
| [Find](../../aspose.cells/cells/find/#find_1)(object, Cell, FindOptions) | Encuentra la celda que contiene el objeto de entrada. |
| [GetCell](../../aspose.cells/cells/getcell/)(int, int) | (**Obsoleto.**) Obtiene el elemento [`Cell`](../cell/) o null en el índice de fila y columna de celda especificados. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle)(int, int) | Obtiene el estilo de visualización de la celda dada. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle_1)(int, int, BorderType) | Obtiene el estilo de visualización de la celda dada. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle/)(int, int) | Obtiene el estilo de la celda dada. |
| [GetCellsWithPlaceInCellPicture](../../aspose.cells/cells/getcellswithplaceincellpicture/)() | Obtiene todas las celdas que contienen una imagen incrustada. |
| [GetColumnOriginalWidthPoint](../../aspose.cells/cells/getcolumnoriginalwidthpoint/)(int) | (**Obsoleto.**) Obtiene la altura original de la columna en unidades de punto si la columna está oculta |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth)(int) | Obtiene el ancho (en unidades de caracteres) de la columna especificada en vista normal |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth_1)(int, bool, CellsUnitType) | Obtiene el ancho de la columna. |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch/)(int) | (**Obsoleto.**) Obtiene el ancho de la columna especificada en vista normal, en unidades de pulgadas. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel)(int) | Obtiene el ancho de la columna especificada en vista normal, en unidades de píxel. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel_1)(int, bool) | (**Obsoleto.**) Obtiene el ancho de la columna especificada en vista normal, en unidades de píxel. |
| [GetDependents](../../aspose.cells/cells/getdependents/)(bool, int, int) | Obtiene todas las celdas que hacen referencia a la celda específica. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation/)(int, int, bool) | Obtiene todas las celdas cuyo resultado calculado depende de la celda específica. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator/)() | Obtiene el enumerador de celdas. |
| [GetFirstDataRow](../../aspose.cells/cells/getfirstdatarow/)(int) | Obtiene el índice de la primera fila de la celda que contiene datos en la columna especificada. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel/)(int) | Obtiene el nivel de esquema (basado en cero) de la columna. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel/)(int) | Obtiene el nivel de esquema (basado en cero) de la fila. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow/)(int) | Obtiene el índice de la última fila de la celda que contiene datos en la columna especificada. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/)() | Obtiene el nivel máximo de esquema de columna agrupada (basado en cero). |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel/)() | Obtiene el nivel máximo de esquema de fila agrupada (basado en cero). |
| [GetMergedAreas](../../aspose.cells/cells/getmergedareas/)() | Obtiene todas las celdas combinadas. |
| [GetRow](../../aspose.cells/cells/getrow/)(int) | (**Obsoleto.**) Obtiene el elemento [`Row`](../row/) en el índice de fila de celda especificado. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator/)() | (**Obsoleto.**) Obtiene el enumerador de filas. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight)(int) | Obtiene la altura de una fila especificada, en unidades de puntos. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight_1)(int, bool, CellsUnitType) | Obtiene la altura de la fila. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch/)(int) | Obtiene la altura de una fila especificada en unidades de pulgadas. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel/)(int) | Obtiene la altura de una fila especificada en unidades de píxel. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint/)(int) | (**Obsolete.**) Obtiene la altura original de la fila en unidades de punto si la fila está oculta |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel/)(int) | Obtiene el ancho en diferentes tipos de vista. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight/)(int) | Obtiene la altura de una fila especificada. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch/)(int) | Obtiene la altura de una fila especificada en unidades de pulgadas. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns)(int, int) | Agrupa columnas. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns_1)(int, int, bool) | Agrupa columnas. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows)(int, int) | Agrupa filas. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows_1)(int, int, bool) | Agrupa filas. |
| [HideColumn](../../aspose.cells/cells/hidecolumn/)(int) | Oculta una columna. |
| [HideColumns](../../aspose.cells/cells/hidecolumns/)(int, int) | Oculta varias columnas. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail/)(bool, int) | Contrae las filas/columnas agrupadas. |
| [HideRow](../../aspose.cells/cells/hiderow/)(int) | Oculta una fila. |
| [HideRows](../../aspose.cells/cells/hiderows/)(int, int) | Oculta varias filas. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_1)(double[], int, int, bool) | Importa una matriz de double a una hoja de cálculo. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_3)(int[], int, int, bool) | Importa una matriz de integer a una hoja de cálculo. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_5)(string[], int, int, bool) | Importa una matriz de string a una hoja de cálculo. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist/)(ArrayList, int, int, bool) | Importa una arraylist de datos a una hoja de cálculo. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv)(Stream, TxtLoadOptions, int, int) | Importa un archivo CSV a las celdas. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_2)(string, TxtLoadOptions, int, int) | Importa un archivo CSV a las celdas. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_1)(Stream, string, bool, int, int) | Importa un archivo CSV a las celdas. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_3)(string, string, bool, int, int) | Importa un archivo CSV a las celdas. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects)(ICollection, int, int, ImportTableOptions) | Importa objetos personalizados. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | Importa objetos personalizados. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_3)(IDataReader, int, int) | Importa datos de un objeto IDataReader. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_1)(DataTable, int, int, ImportTableOptions) | Importa datos de una tabla de datos personalizada. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_2)(DataView, int, int, ImportTableOptions) | Importa datos de una vista de datos. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata)(ICellsDataTable, int, int, ImportTableOptions) | Importa datos de una tabla de datos personalizada. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_4)(IDataReader, int, int, ImportTableOptions) | Importa datos de un objeto IDataReader. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid)(DataGrid, int, int, bool) | Importa un DataGrid a una hoja de cálculo. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_1)(DataGrid, int, int, int, int, bool) | Importa un DataGrid a una hoja de cálculo. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | Importa un DataGrid a una hoja de cálculo. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring/)(DataGrid, int, int, bool) | Importa un DataGrid a una hoja de cálculo. Este método no intenta convertir texto en valores numéricos. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow/)(DataRow, int, int) | Importa un DataRow al archivo Excel. |
| [ImportDataView](../../aspose.cells/cells/importdataview/)(DataView, int, int) | Importa un DataView a una hoja de cálculo. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray/)(string[], int, int, bool) | Importa una matriz de formula a una hoja de cálculo. |
| [ImportGridView](../../aspose.cells/cells/importgridview/)(GridView, int, int, ImportTableOptions) | Importa una vista de cuadrícula a estas celdas. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray)(object[], int, int, bool) | Importa una matriz de datos en una hoja de cálculo. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray_1)(object[], int, int, bool, int) | Importa una matriz de datos en una hoja de cálculo. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn)(int) | Inserta una nueva columna en la hoja de cálculo. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn_1)(int, bool) | Inserta una nueva columna en la hoja de cálculo. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns)(int, int) | Inserta algunas columnas en la hoja de cálculo. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_2)(int, int, bool) | Inserta algunas columnas en la hoja de cálculo. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_1)(int, int, InsertOptions) | Inserta algunas columnas en la hoja de cálculo. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells/)(Range, int, int, ShiftType) | Insertar rango recortado. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange)(CellArea, ShiftType) | Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_1)(CellArea, int, ShiftType) | Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_2)(CellArea, int, ShiftType, bool) | Inserta un rango de celdas y desplaza las celdas según la opción de desplazamiento. |
| [InsertRow](../../aspose.cells/cells/insertrow/)(int) | Inserta una nueva fila en la hoja de cálculo. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows)(int, int) | Inserta varias filas en la hoja de cálculo. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_2)(int, int, bool) | Inserta varias filas en la hoja de cálculo. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_1)(int, int, InsertOptions) | Inserta varias filas en la hoja de cálculo. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn/)(int) | Comprueba si la columna dada está vacía (no contiene datos). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden/)(int) | Comprueba si una columna en el índice dado está oculta. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled/)(int, int, int, int) | Comprueba si el rango puede ser eliminado. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden/)(int) | Comprueba si una fila en el índice dado está oculta. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap/)(string, int, int, string) | Enlace a un mapa XML. |
| [Merge](../../aspose.cells/cells/merge/#merge)(int, int, int, int) | Fusiona un rango especificado de celdas en una sola celda. |
| [Merge](../../aspose.cells/cells/merge/#merge_1)(int, int, int, int, bool) | Fusiona un rango especificado de celdas en una sola celda. |
| [Merge](../../aspose.cells/cells/merge/#merge_2)(int, int, int, int, bool, bool) | Fusiona un rango especificado de celdas en una sola celda. |
| [MoveRange](../../aspose.cells/cells/moverange/)(CellArea, int, int) | Mueve el rango. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates)() | Elimina filas duplicadas en la hoja. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_1)(int, int, int, int) | Elimina valores duplicados en el rango. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_2)(int, int, int, int, bool, int[]) | Elimina datos duplicados del rango. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas/)() | Elimina todas las fórmulas y las reemplaza con el valor de la fórmula. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting/)(CellArea) | Recupera la configuración de subtotales del rango. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth/)(int, double) | Establece el ancho de la columna especificada en vista normal. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch/)(int, double) | Establece el ancho de la columna en unidades de pulgadas en vista normal. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel/)(int, int) | Establece el ancho de la columna en unidades de píxeles en vista normal. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight/)(int, double) | Establece la altura de la fila especificada. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch/)(int, double) | Establece la altura de la fila en unidades de pulgadas. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel/)(int, int) | Establece la altura de la fila en unidades de píxeles. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel/)(int, int) | Establece el ancho de la columna en diferentes vistas. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail/)(bool, int) | Expande las filas/columnas agrupadas. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal)(CellArea, int, ConsolidationFunction, int[]) | Crea subtotales para el rango. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Crea subtotales para el rango. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns/)(int, int, int, TxtLoadOptions) | Divide el contenido en la columna especificada en múltiples columnas.. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns/)(int, int) | Desagrupa columnas. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows)(int, int) | Desagrupa filas. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows_1)(int, int, bool) | Desagrupa filas. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn/)(int, double) | Muestra una columna |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns/)(int, int, double) | Muestra varias columnas. |
| [UnhideRow](../../aspose.cells/cells/unhiderow/)(int, double) | Muestra una fila. |
| [UnhideRows](../../aspose.cells/cells/unhiderows/)(int, int, double) | Muestra las filas ocultas. |
| [UnMerge](../../aspose.cells/cells/unmerge/)(int, int, int, int) | Descombina un rango especificado de celdas combinadas. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsDemo
    {
        public static void CellsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer altura predeterminada de la fila
            cells.StandardHeight = 20;
            // Establecer altura de la fila
            cells.SetRowHeight(2, 20.5);

            // Establecer ancho predeterminado de la columna
            cells.StandardWidth = 15;
            // Establecer ancho de la columna
            cells.SetColumnWidth(3, 12.57);

            // Combinar celdas
            cells.Merge(5, 4, 2, 2);

            // Asignar valores a las celdas
            cells[0, 0].PutValue(true);
            cells[0, 1].PutValue(1);
            cells[0, 2].PutValue("abc");

            // Exportar datos
            object[,] arr = cells.ExportArray(0, 0, 10, 10);

            // Demostrar algunas propiedades
            Console.WriteLine("Total Cells Count: " + cells.Count);
            Console.WriteLine("Total Cells Count (Large): " + cells.CountLarge);
            Console.WriteLine("Min Row with Data: " + cells.MinDataRow);
            Console.WriteLine("Max Row with Data: " + cells.MaxDataRow);
            Console.WriteLine("Min Column with Data: " + cells.MinDataColumn);
            Console.WriteLine("Max Column with Data: " + cells.MaxDataColumn);

            // Iterar a través de celdas
            IEnumerator enumerator = cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Guarda el libro de trabajo
            workbook.Save("CellsExample.xlsx");
            workbook.Save("CellsExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


