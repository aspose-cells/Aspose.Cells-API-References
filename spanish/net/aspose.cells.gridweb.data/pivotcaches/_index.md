---
title: "Clase PivotCaches"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.Data.PivotCaches. Representa la colección de cachés de memoria de los informes PivotTable en un libro. Cada caché de memoria está representado por un objeto PivotCache."
type: docs
url: /es/net/aspose.cells.gridweb.data/pivotcaches/
---
## PivotCaches class

Representa la colección de cachés de memoria de los informes PivotTable en un libro. Cada caché de memoria está representado por un objeto [`PivotCache`](../pivotcache/) .

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotCaches : ICollection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotcaches/count/) { get; } | Obtiene el número de elementos contenidos en la instancia de PivotCaches. |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotcaches/issynchronized/) { get; } | Obtiene un valor que indica si el acceso a los PivotCaches está sincronizado (thread-safe). |
| [Item](../../aspose.cells.gridweb.data/pivotcaches/item/) { get; } | Obtiene el objeto PivotCache por índice. (2 indexadores) |
| [Parent](../../aspose.cells.gridweb.data/pivotcaches/parent/) { get; } | Obtiene el objeto padre para el objeto especificado. Solo lectura. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotcaches/syncroot/) { get; } | Obtiene un objeto que puede usarse para sincronizar el acceso a los PivotCaches. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_2)(DataTable) | Agrega un PivotCache desde DataTable. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_4)(DataView) | Agrega un PivotCache desde DataView. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_3)(DataTable, string) | Agrega un PivotCahe desde DataTable usando el nombre especificado. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_5)(DataView, string) | Agrega un PivotCahe desde DataView usando el nombre especificado. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add)(WebWorksheet, WebCellArea) | Agrega un PivotCache desde la hoja. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_1)(WebWorksheet, WebCellArea, string) | Agrega un PivotCache desde la hoja usando el nombre especificado. |
| [Clear](../../aspose.cells.gridweb.data/pivotcaches/clear/)() | Elimina todos los objetos PivotCache y todos los objetos PivotTable en el control. |
| [CopyTo](../../aspose.cells.gridweb.data/pivotcaches/copyto/)(Array, int) | Copia todo el PivotCache a un Array unidimensional compatible, comenzando en el índice especificado del array de destino. |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotcaches/getenumerator/)() | Devuelve un IEnumerator para los PivotCaches. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotcaches/indexof/)(PivotCache) | Devuelve el índice del PivotCache especificado en la colección. |
| [Remove](../../aspose.cells.gridweb.data/pivotcaches/remove/)(PivotCache) | Elimina el objeto PivotCache especificado de los PivotCaches y la PivotTable relacionada usando el pivotCache como fuente de datos. |
| [RemoveAt](../../aspose.cells.gridweb.data/pivotcaches/removeat/)(int) | Elimina el objeto PivotCache especificado de los PivotCaches y la PivotTable relacionada usando el pivotCache como fuente de datos. |

### Observaciones

NOTA: Esta clase está ahora obsoleta. Por favor, use GridPivotTableCollection en su lugar. Esta clase será eliminada después de 6 meses desde agosto de 2014. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp

 [C#]

 //Suponiendo que la hoja de cálculo "Sheet1" tiene datos, entonces crea un informe PivotTable basado en ella.
 WebWorksheet sourceSheet = GridWeb1.WebWorksheets["Sheet1"];
 Aspose.Cells.GridWeb.Data.WebCellArea sourceRange = new WebCellArea();
 sourceRange.StartRow = 0;
 sourceRange.StartColumn = 0;
 sourceRange.EndRow = 10;
 sourceRange.EndColumn = 5;

 PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(sourceSheet, sourceRange);

 PivotTable table = cache.CreatePivotTable();

 table.PivotFields[0].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[1].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[2].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[3].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;
 table.PivotFields[4].Orientation = PivotFieldOrientation.ColumnField;
 table.PivotFields[5].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;

 table.PivotFields[3].Function = PivotFieldFunction.Count;
 table.PivotFields[5].Function = PivotFieldFunction.Sum;

 table.DataBind();

 //Crea un informe PivotTable a partir de DataView o DataTable.
 DataView dataView;//Or  DataTable dataTable;
     .
     .
     .
 Sets dataView(dataTable) Value
     .
     .
     .

 PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataView);
 //Or PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataTable);
 PivotTable table = cache.CreatePivotTable();
 table = GridWeb1.WebWorksheets.PivotTables["PivotTable1"];
 table.PivotFields[0].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[1].Orientation = PivotFieldOrientation.RowField;
 table.PivotFields[2].Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField;
 table.DataBind();


 [VB]


 'On the assumption that worksheet "Sheet1" has datas, then creates a PivotTable report base on it.
 Dim sourceSheet As WebWorksheet =  GridWeb1.WebWorksheets("Sheet1")
 Dim sourceRange As Aspose.Cells.GridWeb.Data.WebCellArea =  New WebCellArea()/
 sourceRange.StartRow = 0
 sourceRange.StartColumn = 0
 sourceRange.EndRow = 10
 sourceRange.EndColumn = 5

 Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(sourceSheet,sourceRange)

 Dim table As PivotTable =  cache.CreatePivotTable()

 table.PivotFields(0).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(1).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(2).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(3).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField
 table.PivotFields(4).Orientation = PivotFieldOrientation.ColumnField
 table.PivotFields(5).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField

 table.PivotFields(3).Function = PivotFieldFunction.Count
 table.PivotFields(5).Function = PivotFieldFunction.Sum

 table.DataBind()

 'Creates a PivotTable report from DataView or DataTable.

 Dim dataView As DataView ' Or Dim dataTable As DataTable
     .
     .
 Sets dataView(dataTable) Value
     .
     .
     .

 Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(dataView)
 'Or Dim cache As PivotCache =  GridWeb1.WebWorksheets.PivotCaches.Add(dataTable)
 Dim table As PivotTable =  cache.CreatePivotTable()
 table = GridWeb1.WebWorksheets.PivotTables("PivotTable1")
 table.PivotFields(0).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(1).Orientation = PivotFieldOrientation.RowField
 table.PivotFields(2).Orientation = PivotFieldOrientation.ColumnField | PivotFieldOrientation.DataField
 table.DataBind()

```

### Ver también

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


