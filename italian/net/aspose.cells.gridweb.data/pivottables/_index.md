---
title: "Classe PivotTables"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.PivotTables. Rappresenta una collezione di tutti gli oggetti PivotTable."
type: docs
url: /it/net/aspose.cells.gridweb.data/pivottables/
---
## PivotTables class

Rappresenta una collezione di tutti gli oggetti [`PivotTable`](../pivottable/).

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotTables : ICollection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivottables/count/) { get; } | Ottiene il numero di elementi contenuti nell'istanza PivotTables. |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivottables/issynchronized/) { get; } | Ottiene un valore che indica se l'accesso a PivotTables è sincronizzato (thread-safe). |
| [Item](../../aspose.cells.gridweb.data/pivottables/item/) { get; } | Ottiene un oggetto PivotTable per indice. (2 indicizzatori) |
| [Parent](../../aspose.cells.gridweb.data/pivottables/parent/) { get; } | Ottiene l'oggetto padre per l'oggetto specificato. Sola lettura. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivottables/syncroot/) { get; } | Ottiene un oggetto che può essere utilizzato per sincronizzare l'accesso a PivotTables. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add)(PivotCache) | Aggiunge un oggetto PivotTable dal PivotCache specificato a un nuovo foglio di lavoro. |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_3)(PivotCache, string) | Aggiunge un oggetto PivotTable dal PivotCache specificato a un nuovo foglio di lavoro. |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_1)(PivotCache, WebWorksheet, WebCell) | Aggiunge un oggetto PivotTable dal PivotCache specificato al foglio di lavoro specificato. |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_2)(PivotCache, WebWorksheet, WebCell, string) | Aggiunge un oggetto PivotTable dal PivotCache specificato al foglio di lavoro specificato. |
| [Clear](../../aspose.cells.gridweb.data/pivottables/clear/)() | Rimuove tutti gli oggetti PivotTable e tutti gli oggetti PivotCache nel controllo. |
| [Contains](../../aspose.cells.gridweb.data/pivottables/contains/)(string) | Restituisce true se esiste un nome di PivotTable tableName. |
| [CopyTo](../../aspose.cells.gridweb.data/pivottables/copyto/)(Array, int) | Copia l'intera PivotTable in un Array monodimensionale compatibile, iniziando all'indice specificato dell'array di destinazione |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivottables/getenumerator/)() | Restituisce un IEnumerator per le PivotTables. |
| [Refresh](../../aspose.cells.gridweb.data/pivottables/refresh/)(PivotTable) | ReDataBinds la fonte dati al report della PivotTable. |
| [RefreshAll](../../aspose.cells.gridweb.data/pivottables/refreshall/)() | ReDataBinds la fonte dati a tutti i report della PivotTable. |
| [Remove](../../aspose.cells.gridweb.data/pivottables/remove/)(PivotTable) | Rimuove l'oggetto PivotTable specificato dalle PivotTables e dal relativo PivotCache se non è utilizzato da altre PivotTable |
| [RemoveAt](../../aspose.cells.gridweb.data/pivottables/removeat/)(int) | Rimuove l'oggetto PivotTable specificato dalle PivotTables e dal relativo PivotCache se non è utilizzato da altre PivotTable |

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


