---
title: "Clase WorksheetCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.WorksheetCollection. Encapsula una colección de objetos Worksheet"
type: docs
url: /es/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Encapsula una colección de objetos [`Worksheet`](../worksheet/).

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex/) { get; set; } | Representa el índice de la hoja de cálculo activa cuando se abre la hoja de cálculo. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname/) { get; set; } | Representa el nombre de la hoja de cálculo activa cuando se abre la hoja de cálculo. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties/) { get; } | Devuelve una colección de [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) que representa todas las propiedades de documento incorporadas de la hoja de cálculo. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties/) { get; } | Devuelve una colección de [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) que representa todas las propiedades de documento personalizadas de la hoja de cálculo. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs/) { get; } | Obtiene los registros maestros de formato diferencial. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks/) { get; } | Representa enlaces externos en un libro de trabajo. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections/) { get; set; } | Indica si se deben actualizar todas las conexiones al abrir el archivo en MS Excel. |
| [Item](../../aspose.cells/worksheetcollection/item/) { get; } | Obtiene el elemento [`Worksheet`](../worksheet/) en el índice especificado. (2 indexadores) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names/) { get; } | Obtiene la colección de todos los objetos Name en la hoja de cálculo. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize/) { get; set; } | Obtiene y establece el tamaño mostrado cuando el archivo Workbook se usa como un objeto Ole. |
| [PivotCaches](../../aspose.cells/worksheetcollection/pivotcaches/) { get; } | Obtiene todos los [`PivotCache`](../../aspose.cells.pivot/pivotcache/). |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs/) { get; } | Representa los registros de revisiones. |
| [SensitivityLabels](../../aspose.cells/worksheetcollection/sensitivitylabels/) { get; } | Representa todas las etiquetas de sensibilidad. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles/) { get; } | Obtiene el objeto [`TableStyles`](./tablestyles/). |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors/) { get; } | Obtiene la lista de autores de comentarios en hilo. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions/) { get; } | Obtiene la lista de paneles de tareas. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes/) { get; } | Obtiene la lista de paneles de tareas. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps/) { get; set; } | Obtiene y establece los mapas XML en el libro de trabajo. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add/#add_1)() | Agrega una hoja de cálculo a la colección. |
| [Add](../../aspose.cells/worksheetcollection/add/#add_2)(SheetType) | Agrega una hoja de cálculo a la colección. |
| [Add](../../aspose.cells/worksheetcollection/add/#add)(string) | Agrega una hoja de cálculo a la colección. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy)(int) | Agrega una hoja de cálculo a la colección y copia datos de una hoja de cálculo existente. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_1)(string) | Agrega una hoja de cálculo a la colección y copia datos de una hoja de cálculo existente. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_2)(Worksheet[], string[]) | Copiar un grupo de hojas de cálculo. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear/#clear)() | Borrar todas las hojas de cálculo. (2 métodos) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables/)() | Borra las tablas dinámicas de la hoja de cálculo. |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange/)(string, int) | Crea un objeto [`Range`](../range/) a partir de una dirección del rango. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange/)(string, int) | Crea un objeto [`Range`](../range/) a partir de una dirección del rango. |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges/)() | Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables/)() | Obtiene todos los rangos con nombre predefinidos en la hoja de cálculo. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname)(string) | Obtiene el objeto Range por nombre predefinido. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname_1)(string, int, bool) | Obtiene [`Range`](../range/) por nombre predefinido o nombre de tabla |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename/)(string) | Obtiene la hoja de cálculo por el nombre de código. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert)(int, SheetType) | Insertar una hoja de cálculo. |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert_1)(int, SheetType, string) | Insertar una hoja de cálculo. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int, int) |  |
| [RefreshAll](../../aspose.cells/worksheetcollection/refreshall/)() | (**Obsoleto.**) Actualiza todas las tablas dinámicas y gráficos con la fuente de pivote. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables_1)() | Actualiza todas las PivotTables en el archivo Excel. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables)(PivotTableRefreshOption) | Actualiza todas las PivotTables en el archivo Excel. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction_1)(int, string) | Agrega la función de complemento al libro de trabajo |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction)(string, string, bool) | Agrega la función de complemento al libro de trabajo |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat)(int) | Elimina el elemento en un índice especificado. (2 métodos) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat_2)(string) | Elimina el elemento con un nombre especificado. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize/)(int, int, int, int) | Establece el tamaño mostrado cuando el archivo Workbook se usa como objeto Ole. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames/)() | Ordena los nombres definidos. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet/)(int, int) | Intercambia las dos hojas. |

### Ejemplos

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionDemo
    {
        public static void RunDemo()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;

            // Agregar una nueva hoja de cálculo a la colección
            int newSheetIndex = worksheets.Add(SheetType.Worksheet);
            Worksheet newSheet = worksheets[newSheetIndex];
            newSheet.Name = "NewSheet";

            // Acceder a una hoja de cálculo existente por índice
            Worksheet firstSheet = worksheets[0];
            firstSheet.Name = "FirstSheet";

            // Acceder a una hoja de cálculo existente por nombre
            Worksheet retrievedSheet = worksheets["FirstSheet"];

            // Establecer la hoja activa
            worksheets.ActiveSheetIndex = newSheetIndex;

            // Establecer el nombre de la hoja activa
            worksheets.ActiveSheetName = "NewSheet";

            // Actualizar todas las tablas dinámicas en el libro de trabajo
            worksheets.RefreshAll();

            // Borrar todas las tablas dinámicas del libro de trabajo
            worksheets.ClearPivottables();

            // Guarda el libro de trabajo
            workbook.Save("WorksheetCollectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Worksheet](../worksheet/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


