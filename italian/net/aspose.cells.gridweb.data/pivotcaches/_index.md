---
title: "Classe PivotCaches"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.PivotCaches. Rappresenta la collezione di cache di memoria dai report PivotTable in una cartella di lavoro. Ogni cache di memoria è rappresentata da un oggetto PivotCache."
type: docs
url: /it/net/aspose.cells.gridweb.data/pivotcaches/
---
## PivotCaches class

Rappresenta la collezione di cache di memoria dai report PivotTable in una cartella di lavoro. Ogni cache di memoria è rappresentata da un oggetto [`PivotCache`](../pivotcache/).

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotCaches : ICollection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotcaches/count/) { get; } | Restituisce il numero di elementi contenuti nell'istanza PivotCaches |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotcaches/issynchronized/) { get; } | Restituisce un valore che indica se l'accesso a PivotCaches è sincronizzato (thread-safe). |
| [Item](../../aspose.cells.gridweb.data/pivotcaches/item/) { get; } | Restituisce l'oggetto PivotCache per indice. (2 indicizzatori) |
| [Parent](../../aspose.cells.gridweb.data/pivotcaches/parent/) { get; } | Ottiene l'oggetto padre per l'oggetto specificato. Sola lettura. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotcaches/syncroot/) { get; } | Restituisce un oggetto che può essere usato per sincronizzare l'accesso a PivotCaches. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_2)(DataTable) | Aggiunge un PivotCache da DataTable. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_4)(DataView) | Aggiunge un PivotCache da DataView. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_3)(DataTable, string) | Aggiunge un PivotCahe da DataTable usando il nome specificato. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_5)(DataView, string) | Aggiunge un PivotCahe da DataView usando il nome specificato. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add)(WebWorksheet, WebCellArea) | Aggiunge un PivotCache da foglio |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_1)(WebWorksheet, WebCellArea, string) | Aggiunge un PivotCache da foglio usando il nome specificato. |
| [Clear](../../aspose.cells.gridweb.data/pivotcaches/clear/)() | Rimuove tutti gli oggetti PivotCache e tutti gli oggetti PivotTable nel controllo. |
| [CopyTo](../../aspose.cells.gridweb.data/pivotcaches/copyto/)(Array, int) | Copia l'intero PivotCache in un Array monodimensionale compatibile, iniziando dall'indice specificato dell'array di destinazione. |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotcaches/getenumerator/)() | Restituisce un IEnumerator per i PivotCaches. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotcaches/indexof/)(PivotCache) | Restituisce l'indice del PivotCache specificato nella collezione. |
| [Remove](../../aspose.cells.gridweb.data/pivotcaches/remove/)(PivotCache) | Rimuove l'oggetto PivotCache specificato dai PivotCaches e dalla PivotTable correlata usando il pivotCache come origine dati. |
| [RemoveAt](../../aspose.cells.gridweb.data/pivotcaches/removeat/)(int) | Rimuove l'oggetto PivotCache specificato dai PivotCaches e dalla PivotTable correlata usando il pivotCache come origine dati. |

### Osservazioni

NOTA: Questa classe è ora obsoleta. si prega di utilizzare GridPivotTableCollection invece. Questa classe sarà rimossa dopo 6 mesi da agosto 2014. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp

 [C#]

 //Assumendo che il foglio di lavoro "Sheet1" contenga dati, crea quindi un report PivotTable basato su di esso.
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

 //Crea un report PivotTable da DataView o DataTable.
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

### Vedi anche

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


