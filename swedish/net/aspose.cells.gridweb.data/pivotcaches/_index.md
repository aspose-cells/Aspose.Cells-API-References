---
title: "Klass PivotCaches"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.PivotCaches-klass. Representerar samlingen av minnescache från PivotTable-rapporter i en arbetsbok. Varje minnescache representeras av ett PivotCache-objekt."
type: docs
url: /sv/net/aspose.cells.gridweb.data/pivotcaches/
---
## PivotCaches class

Representerar samlingen av minnescache från PivotTable-rapporter i en arbetsbok. Varje minnescache representeras av ett [`PivotCache`](../pivotcache/) objekt.

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotCaches : ICollection
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotcaches/count/) { get; } | Hämtar antalet element som finns i PivotCaches-instansen. |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotcaches/issynchronized/) { get; } | Hämtar ett värde som indikerar om åtkomst till PivotCaches är synkroniserad (trådsäker). |
| [Item](../../aspose.cells.gridweb.data/pivotcaches/item/) { get; } | Hämtar PivotCache-objekt efter index. (2 indexerare) |
| [Parent](../../aspose.cells.gridweb.data/pivotcaches/parent/) { get; } | Hämtar föräldraobjektet för det angivna objektet. Skrivskyddad. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotcaches/syncroot/) { get; } | Hämtar ett objekt som kan användas för att synkronisera åtkomst till PivotCaches. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_2)(DataTable) | Lägger till en PivotCache från DataTable. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_4)(DataView) | Lägger till en PivotCache från DataView. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_3)(DataTable, string) | Lägger till en PivotCahe från DataTable med det angivna namnet. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_5)(DataView, string) | Lägger till en PivotCahe från DataView med det angivna namnet. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add)(WebWorksheet, WebCellArea) | Lägger till en PivotCache från blad |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_1)(WebWorksheet, WebCellArea, string) | Lägger till en PivotCache från blad med det angivna namnet. |
| [Clear](../../aspose.cells.gridweb.data/pivotcaches/clear/)() | Tar bort alla PivotCache-objekt och alla PivotTable-objekt i kontrollen. |
| [CopyTo](../../aspose.cells.gridweb.data/pivotcaches/copyto/)(Array, int) | Kopierar hela PivotCache till en kompatibel endimensionell Array, med start vid det angivna indexet i målarrayen |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotcaches/getenumerator/)() | Returnerar en IEnumerator för PivotCaches. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotcaches/indexof/)(PivotCache) | Returnerar indexet för den angivna PivotCache i samlingen |
| [Remove](../../aspose.cells.gridweb.data/pivotcaches/remove/)(PivotCache) | Tar bort det angivna PivotCache-objektet från PivotCaches och den relaterade PivotTable som använder pivotCache som datakälla. |
| [RemoveAt](../../aspose.cells.gridweb.data/pivotcaches/removeat/)(int) | Tar bort det angivna PivotCache-objektet från PivotCaches och den relaterade PivotTable som använder pivotCache som datakälla. |

### Anmärkningar

OBS: Denna klass är nu föråldrad. använd GridPivotTableCollection istället. Denna klass kommer att tas bort efter 6 månader från augusti 2014. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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


