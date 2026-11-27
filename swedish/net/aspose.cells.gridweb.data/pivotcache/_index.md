---
title: "Klass PivotCache"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.PivotCache klass. Representerar minnescachen för en PivotTable-rapport. PivotCache-objektet är en medlem i PivotCaches-samlingen"
type: docs
url: /sv/net/aspose.cells.gridweb.data/pivotcache/
---
## PivotCache class

Representerar minnescachen för en PivotTable-rapport. PivotCache-objektet är en medlem i samlingen [`PivotCaches`](../pivotcaches/).

```csharp
[Obsolete("This class is obsolete; use GridPivotTable instead")]
public class PivotCache
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [DataTable](../../aspose.cells.gridweb.data/pivotcache/datatable/) { get; } | Returnerar datakällan för System.Data.DataTable för PivotTable-rapporten. |
| [DataView](../../aspose.cells.gridweb.data/pivotcache/dataview/) { get; } | Returnerar datakällan för System.Data.DataView för PivotTable-rapporten. |
| [Index](../../aspose.cells.gridweb.data/pivotcache/index/) { get; } | Returnerar indexet för detta objekt i Parent |
| [Name](../../aspose.cells.gridweb.data/pivotcache/name/) { get; } | Returnerar namnet på PivotCache.Re |
| [Parent](../../aspose.cells.gridweb.data/pivotcache/parent/) { get; } | Returnerar föräldraobjektet för det angivna objektet (behållaren för PivotCache). Endast läsning. |
| [SourceCellArea](../../aspose.cells.gridweb.data/pivotcache/sourcecellarea/) { get; } | Returnerar intervallet för datakällan som används med SourceSheet. |
| [SourceSheet](../../aspose.cells.gridweb.data/pivotcache/sourcesheet/) { get; } | Returnerar datakällan för WebWorksheet för PivotTable-rapporten. |
| [SourceType](../../aspose.cells.gridweb.data/pivotcache/sourcetype/) { get; } | Representerar typen av källdata |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable)() | Skapar en PivotTable-rapport till ett nytt blad. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_3)(string) | Skapar en PivotTable-rapport till ett nytt blad. Namnet på pivotTable-objektet |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_1)(WebWorksheet, WebCell) | Skapar en PivotTable-rapport till targetSheet. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_2)(WebWorksheet, WebCell, string) | Skapar en PivotTable-rapport till targetSheet. |
| override [Equals](../../aspose.cells.gridweb.data/pivotcache/equals/)(object) | Bestämmer om två Object-instans är lika. |
| override [GetHashCode](../../aspose.cells.gridweb.data/pivotcache/gethashcode/)() | Fungerar som en hashfunktion för en viss typ, lämplig för användning i hashalgoritmer och datastrukturer som en hashtabell. |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_1)(DataTable) | Återställer källdata |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_2)(DataView) | Återställer källdata |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource)(WebWorksheet, WebCellArea) | Återställer källdata |
| override [ToString](../../aspose.cells.gridweb.data/pivotcache/tostring/)() | Returnerar en String som representerar det aktuella objektet |

### Anmärkningar

OBS: Den här klassen är nu föråldrad. vänligen använd GridPivotTable istället. Den här klassen kommer att tas bort efter 6 månader från augusti 2014. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

Använder PivotCache‑metoden för att returnera ett PivotCache‑objekt för en PivotTable‑rapport (varje rapport har bara en cache). Källdata för PivotCache kommer från WebWorksheet, DataTable och så vidare.

### Exempel

```csharp

 [C#]

 //Under antagandet att kalkylbladet "Sheet1" har data, skapas en PivotTable‑rapport baserad på den.
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

 //Skapar en PivotTable‑rapport från DataView eller DataTable.
 DataView dataView;//Or  DataTable dataTable;
     .
     .
     .
 Sets dataView(dataTable) Value
     .
     .
     .

 PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataView);
 //Eller PivotCache cache = GridWeb1.WebWorksheets.PivotCaches.Add(dataTable);
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

### Se även

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


