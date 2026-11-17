---
title: "Clase WorksheetCollection"
linktitle: "WorksheetCollection"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase WorksheetCollection. Encapsula el objeto que representa worksheetcollection en Go."
type: docs
weight: 200
url: /es/go-cpp/worksheetcollection/
---

## WorksheetCollection class

Encapsulates a collection of <see cref="Worksheet"/> objects.

```go

type WorksheetCollection struct  {
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
| [GetWebExtensionTaskPanes](./getwebextensiontaskpanes/) | Obtiene la lista de paneles de tareas. |
| [GetWebExtensions](./getwebextensions/) | Obtiene la lista de paneles de tareas. |
| [GetThreadedCommentAuthors](./getthreadedcommentauthors/) | Obtiene la lista de autores de comentarios en hilo. |
| [IsRefreshAllConnections](./isrefreshallconnections/) | Indica si se actualizan todas las conexiones al abrir el archivo en MS Excel. |
| [SetIsRefreshAllConnections](./setisrefreshallconnections/) | Indica si se actualizan todas las conexiones al abrir el archivo en MS Excel. |
| [CreateRange](./createrange/) | Creates a Range object from an address of the range. |
| [CreateUnionRange](./createunionrange/) | Creates a Range object from an address of the range. |
| [GetNames](./getnames/) | Obtiene la colección de todos los objetos Name en la hoja de cálculo. |
| [Get_Int](./get_int/) | Obtiene el elemento Worksheet en el índice especificado. |
| [Get_String](./get_string/) | Obtiene el elemento Worksheet con el nombre especificado. |
| [GetSheetByCodeName](./getsheetbycodename/) | Obtiene la hoja de cálculo por el nombre de código. |
| [GetActiveSheetName](./getactivesheetname/) | Representa el nombre de la hoja activa cuando se abre la hoja de cálculo. |
| [SetActiveSheetName](./setactivesheetname/) | Representa el nombre de la hoja activa cuando se abre la hoja de cálculo. |
| [GetActiveSheetIndex](./getactivesheetindex/) | Representa el índice de la hoja activa cuando se abre la hoja de cálculo. |
| [SetActiveSheetIndex](./setactivesheetindex/) | Representa el índice de la hoja activa cuando se abre la hoja de cálculo. |
| [SortNames](./sortnames/) | Ordena los nombres definidos. |
| [Insert_Int_SheetType](./insert_int_sheettype/) | Inserta una hoja de cálculo. |
| [Insert_Int_SheetType_String](./insert_int_sheettype_string/) | Inserta una hoja de cálculo. |
| [Add_SheetType](./add_sheettype/) | Añade una hoja de cálculo a la colección. |
| [SwapSheet](./swapsheet/) | Intercambia las dos hojas. |
| [Add](./add/) | Añade una hoja de cálculo a la colección. |
| [Add_String](./add_string/) | Añade una hoja de cálculo a la colección. |
| [RegisterAddInFunction_String_String_Bool](./registeraddinfunction_string_string_bool/) | Añade la función addin al libro de trabajo. |
| [RegisterAddInFunction_Int_String](./registeraddinfunction_int_string/) | Añade la función addin al libro de trabajo. |
| [RemoveAt_String](./removeat_string/) | Elimina el elemento con un nombre especificado. |
| [RemoveAt_Int](./removeat_int/) | Elimina el elemento en un índice especificado. |
| [Clear](./clear/) | Borra todas las hojas de cálculo. |
| [AddCopy_String](./addcopy_string/) | Añade una hoja de cálculo a la colección y copia datos de una hoja existente. |
| [AddCopy_Int](./addcopy_int/) | Añade una hoja de cálculo a la colección y copia datos de una hoja existente. |
| [AddCopy_WorksheetArray_stringArray](./addcopy_worksheetarray_stringarray/) | Copia un grupo de hojas de cálculo. |
| [GetDxfs](./getdxfs/) | Obtiene los registros maestros de formato diferencial. |
| [GetRangeByName_String](./getrangebyname_string/) | Obtiene el objeto Range por nombre predefinido. |
| [GetRangeByName_String_Int_Bool](./getrangebyname_string_int_bool/) | Obtiene Range por nombre predefinido o nombre de tabla |
| [GetNamedRanges](./getnamedranges/) | Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo. |
| [GetNamedRangesAndTables](./getnamedrangesandtables/) | Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo. |
| [GetXmlMaps](./getxmlmaps/) | Obtiene y establece los mapas XML en el libro de trabajo. |
| [SetXmlMaps](./setxmlmaps/) | Obtiene y establece los mapas XML en el libro de trabajo. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Returns a DocumentProperty collection that represents all the built-in document properties of the spreadsheet. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Returns a DocumentProperty collection that represents all the custom document properties of the spreadsheet. |
| [GetOleSize](./getolesize/) | Obtiene y establece el tamaño mostrado cuando el archivo Workbook se usa como un objeto Ole. |
| [SetOleSize_Object](./setolesize_object/) | Obtiene y establece el tamaño mostrado cuando el archivo Workbook se usa como un objeto Ole. |
| [SetOleSize_Int_Int_Int_Int](./setolesize_int_int_int_int/) | Establece el tamaño mostrado cuando el archivo Workbook se usa como un objeto Ole. |
| [GetExternalLinks](./getexternallinks/) | Representa enlaces externos en un libro de trabajo. |
| [GetPivotCaches](./getpivotcaches/) | Obtiene todos los PivotCache. |
| [GetTableStyles](./gettablestyles/) | Obtiene el objeto TableStyles. |
| [ClearPivottables](./clearpivottables/) | Elimina las tablas dinámicas de la hoja de cálculo. |
| [GetRevisionLogs](./getrevisionlogs/) | Representa los registros de revisiones. |
| [RefreshPivotTables](./refreshpivottables/) | Actualiza todas las PivotTables en el archivo Excel. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Actualiza todas las PivotTables en el archivo Excel. |
| [GetSensitivityLabels](./getsensitivitylabels/) | Representa todas las etiquetas de sensibilidad. |
| [GetCount](./getcount/) | Gets the number of elements contained in the instance. |
