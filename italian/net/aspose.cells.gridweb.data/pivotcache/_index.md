---
title: "Classe PivotCache"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.PivotCache. Rappresenta la cache di memoria per un report PivotTable. L'oggetto PivotCache è un membro della collezione PivotCaches"
type: docs
url: /it/net/aspose.cells.gridweb.data/pivotcache/
---
## PivotCache class

Rappresenta la cache di memoria per un report PivotTable. L'oggetto PivotCache è un membro della collezione [`PivotCaches`](../pivotcaches/).

```csharp
[Obsolete("This class is obsolete; use GridPivotTable instead")]
public class PivotCache
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DataTable](../../aspose.cells.gridweb.data/pivotcache/datatable/) { get; } | Restituisce l'origine dati di System.Data.DataTable per il report PivotTable. |
| [DataView](../../aspose.cells.gridweb.data/pivotcache/dataview/) { get; } | Restituisce l'origine dati di System.Data.DataView per il report PivotTable. |
| [Index](../../aspose.cells.gridweb.data/pivotcache/index/) { get; } | Restituisce l'indice di questo oggetto nel genitore |
| [Name](../../aspose.cells.gridweb.data/pivotcache/name/) { get; } | Restituisce il nome di PivotCache.Re |
| [Parent](../../aspose.cells.gridweb.data/pivotcache/parent/) { get; } | Restituisce l'oggetto genitore per l'oggetto specificato (il contenitore di PivotCache). Sola lettura. |
| [SourceCellArea](../../aspose.cells.gridweb.data/pivotcache/sourcecellarea/) { get; } | Restituisce l'intervallo dell'origine dati utilizzando SourceSheet. |
| [SourceSheet](../../aspose.cells.gridweb.data/pivotcache/sourcesheet/) { get; } | Restituisce l'origine dati di WebWorksheet per il report PivotTable. |
| [SourceType](../../aspose.cells.gridweb.data/pivotcache/sourcetype/) { get; } | Rappresenta il tipo dei dati di origine |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable)() | Crea un report PivotTable in un nuovo foglio. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_3)(string) | Crea un report PivotTable in un nuovo foglio. Il nome dell'oggetto pivotTable |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_1)(WebWorksheet, WebCell) | Crea un report PivotTable nel foglio di destinazione. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_2)(WebWorksheet, WebCell, string) | Crea un report PivotTable nel foglio di destinazione. |
| override [Equals](../../aspose.cells.gridweb.data/pivotcache/equals/)(object) | Determina se due istanze di Object sono uguali. |
| override [GetHashCode](../../aspose.cells.gridweb.data/pivotcache/gethashcode/)() | Funziona come funzione hash per un tipo specifico, adatta all'uso in algoritmi di hashing e strutture dati come una tabella hash. |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_1)(DataTable) | Reimposta i dati di origine |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_2)(DataView) | Reimposta i dati di origine |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource)(WebWorksheet, WebCellArea) | Reimposta i dati di origine |
| override [ToString](../../aspose.cells.gridweb.data/pivotcache/tostring/)() | Restituisce una String che rappresenta l'Object corrente |

### Osservazioni

NOTA: Questa classe è ora obsoleta. Si prega di utilizzare GridPivotTable invece. Questa classe sarà rimossa dopo 6 mesi da agosto 2014. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

Utilizza il metodo PivotCache per restituire un oggetto PivotCache per un report PivotTable (ogni report ha una sola cache). I dati di origine di PivotCache provengono da WebWorksheet, DataTable e così via.

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


