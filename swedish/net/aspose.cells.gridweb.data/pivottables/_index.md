---
title: "Klass PivotTables"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.PivotTables klass. Representerar en samling av alla PivotTable‑objekt"
type: docs
url: /sv/net/aspose.cells.gridweb.data/pivottables/
---
## PivotTables class

Representerar en samling av alla [`PivotTable`](../pivottable/) objekt

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotTables : ICollection
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivottables/count/) { get; } | Hämtar antalet element som finns i PivotTables‑instansen |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivottables/issynchronized/) { get; } | Hämtar ett värde som indikerar om åtkomst till PivotTables är synkroniserad (trådsäker). |
| [Item](../../aspose.cells.gridweb.data/pivottables/item/) { get; } | Hämtar ett PivotTable‑objekt efter index. (2 indexerare) |
| [Parent](../../aspose.cells.gridweb.data/pivottables/parent/) { get; } | Hämtar föräldraobjektet för det angivna objektet. Skrivskyddad. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivottables/syncroot/) { get; } | Hämtar ett objekt som kan användas för att synkronisera åtkomst till PivotTables. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add)(PivotCache) | Lägger till ett PivotTable‑objekt från den specificerade PivotCache till ett nytt kalkylblad |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_3)(PivotCache, string) | Lägger till ett PivotTable‑objekt från den specificerade PivotCache till ett nytt kalkylblad |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_1)(PivotCache, WebWorksheet, WebCell) | Lägger till ett PivotTable‑objekt från den specificerade PivotCache till det specificerade kalkylbladet |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_2)(PivotCache, WebWorksheet, WebCell, string) | Lägger till ett PivotTable‑objekt från den specificerade PivotCache till det specificerade kalkylbladet |
| [Clear](../../aspose.cells.gridweb.data/pivottables/clear/)() | Tar bort alla PivotTable‑objekt och alla PivotCache‑objekt i kontrollen. |
| [Contains](../../aspose.cells.gridweb.data/pivottables/contains/)(string) | Returnerar true om pivottable‑namnet tableName finns. |
| [CopyTo](../../aspose.cells.gridweb.data/pivottables/copyto/)(Array, int) | Kopierar hela PivotTable till en kompatibel endimensionell Array, med start vid det specificerade indexet i målarrayen |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivottables/getenumerator/)() | Returnerar en IEnumerator för PivotTables. |
| [Refresh](../../aspose.cells.gridweb.data/pivottables/refresh/)(PivotTable) | ReDataBinds datakälla till PivotTable‑rapporten. |
| [RefreshAll](../../aspose.cells.gridweb.data/pivottables/refreshall/)() | ReDataBinds datakälla till alla PivotTable-rapporter. |
| [Remove](../../aspose.cells.gridweb.data/pivottables/remove/)(PivotTable) | Tar bort det angivna PivotTable-objektet från PivotTables och den relaterade PivotCache om det inte används av annan PivotTable. |
| [RemoveAt](../../aspose.cells.gridweb.data/pivottables/removeat/)(int) | Tar bort det angivna PivotTable-objektet från PivotTables och den relaterade PivotCache om det inte används av annan PivotTable. |

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


