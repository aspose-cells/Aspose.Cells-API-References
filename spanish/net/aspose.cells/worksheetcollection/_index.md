---
title: WorksheetCollection
second_title: Referencia de API de Aspose.Cells para .NET
description: Encapsula una colección deWorksheet./worksheet objetos.
type: docs
weight: 6520
url: /es/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Encapsula una colección de[`Worksheet`](../worksheet) objetos.

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex) { get; set; } | Representa el índice de la hoja de cálculo activa cuando se abre la hoja de cálculo. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname) { get; set; } | Representa el nombre de la hoja de cálculo activa cuando se abre la hoja de cálculo. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties) { get; } | Devuelve un[`DocumentProperty`](../../aspose.cells.properties/documentproperty)colección que representa todas las propiedades de documento integradas de la hoja de cálculo. |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties) { get; } | Devuelve un[`DocumentProperty`](../../aspose.cells.properties/documentproperty) colección que representa todas las propiedades del documento personalizado de la hoja de cálculo. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs) { get; } | Obtiene los registros maestros de formato diferencial. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks) { get; } | Representa enlaces externos en un libro de trabajo. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections) { get; set; } | Indica si se actualizan todas las conexiones al abrir el archivo en MS Excel. |
| [Item](../../aspose.cells/worksheetcollection/item) { get; } | Obtiene el[`Worksheet`](../worksheet) elemento en el índice especificado. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names) { get; } | Obtiene la colección de todos los objetos Name en la hoja de cálculo. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize) { get; set; } | Obtiene y establece el tamaño mostrado cuando el archivo Workbook se usa como un objeto Ole. |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs) { get; } | Representa registros de revisión. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles) { get; } | Obtiene[`TableStyles`](./tablestyles) objeto. |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors) { get; } | Obtiene la lista de autores de comentarios encadenados. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions) { get; } | Obtiene la lista de paneles de tareas. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes) { get; } | Obtiene la lista de paneles de tareas. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps) { get; set; } | Obtiene y establece los mapas XML en el libro de trabajo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add#add_1)() | Agrega una hoja de trabajo a la colección. |
| [Add](../../aspose.cells/worksheetcollection/add#add_2)(SheetType) | Agrega una hoja de trabajo a la colección. |
| [Add](../../aspose.cells/worksheetcollection/add#add)(string) | Agrega una hoja de trabajo a la colección. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy)(int) | Agrega una hoja de trabajo a la colección y copia datos de una hoja de trabajo existente. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy_1)(string) | Agrega una hoja de trabajo a la colección y copia datos de una hoja de trabajo existente. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear#clear)() | Borrar todas las hojas de trabajo. (2 methods) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables)() | Borra las tablas dinámicas de la hoja de cálculo. |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange)(string, int) | Crea un[`Range`](../range) objeto de una dirección del rango. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange)(string, int) | Crea un[`Range`](../range) objeto de una dirección del rango. |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges)() | Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables)() | Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname)(string) | Obtiene el objeto Rango por nombre predefinido. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname_1)(string, int, bool) | Obtiene[`Range`](../range) por nombre predefinido o nombre de la tabla |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename)(string) | Obtiene la hoja de trabajo por el nombre del código. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert)(int, SheetType) | Insertar una hoja de trabajo. |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert_1)(int, SheetType, string) | Insertar una hoja de trabajo. |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int, int) |  |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables)() | Actualiza todas las tablas dinámicas en WorksheetCollection. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction_1)(int, string) | Agrega la función addin al libro de trabajo |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction)(string, string, bool) | Agrega la función addin al libro de trabajo |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat)(int) | Elimina el elemento en un índice especificado. (2 methods) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat_2)(string) | Elimina el elemento en un nombre especificado. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize)(int, int, int, int) | Establece el tamaño que se muestra cuando el archivo del libro de trabajo se usa como un objeto Ole. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames)() | Ordena los nombres definidos. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet)(int, int) | Intercambia las dos hojas. |

### Ejemplos

```csharp
[C#]

Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;

//Añadir una hoja de trabajo
sheets.Add();

//Cambiar el nombre de una hoja de trabajo
sheets[0].Name = "First Sheet";

//Establecer la hoja activa en la segunda hoja de trabajo
sheets.ActiveSheetIndex = 1;

	
[Visual Basic]

Dim excel as Workbook = new Workbook()

Dim sheets as WorksheetCollection = excel.Worksheets

'Agregar una hoja de trabajo
sheets.Add()

'Cambiar el nombre de una hoja de trabajo
sheets(0).Name = "First Sheet"

'Establecer la hoja activa en la segunda hoja de trabajo
sheets.ActiveSheetIndex = 1
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Worksheet](../worksheet)
* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
