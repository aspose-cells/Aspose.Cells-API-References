---
title: "Klasse PivotTables"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.PivotTables Klasse. Stellt eine Sammlung aller PivotTable-Objekte dar"
type: docs
url: /de/net/aspose.cells.gridweb.data/pivottables/
---
## PivotTables class

Stellt eine Sammlung aller [`PivotTable`](../pivottable/) Objekte dar

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotTables : ICollection
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivottables/count/) { get; } | Ermittelt die Anzahl der im PivotTables-Instanz enthaltenen Elemente |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivottables/issynchronized/) { get; } | Ermittelt einen Wert, der angibt, ob der Zugriff auf die PivotTables synchronisiert ist (Thread-sicher). |
| [Item](../../aspose.cells.gridweb.data/pivottables/item/) { get; } | Ruft ein PivotTable-Objekt nach Index ab. (2 Indexer) |
| [Parent](../../aspose.cells.gridweb.data/pivottables/parent/) { get; } | Liefert das übergeordnete Objekt für das angegebene Objekt. Nur lesbar. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivottables/syncroot/) { get; } | Ermittelt ein Objekt, das zum Synchronisieren des Zugriffs auf die PivotTables verwendet werden kann. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add)(PivotCache) | Fügt ein PivotTable-Objekt aus dem angegebenen PivotCache zu einem neuen Arbeitsblatt hinzu |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_3)(PivotCache, string) | Fügt ein PivotTable-Objekt aus dem angegebenen PivotCache zu einem neuen Arbeitsblatt hinzu |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_1)(PivotCache, WebWorksheet, WebCell) | Fügt ein PivotTable-Objekt aus dem angegebenen PivotCache zum angegebenen Arbeitsblatt hinzu |
| [Add](../../aspose.cells.gridweb.data/pivottables/add/#add_2)(PivotCache, WebWorksheet, WebCell, string) | Fügt ein PivotTable-Objekt aus dem angegebenen PivotCache zum angegebenen Arbeitsblatt hinzu |
| [Clear](../../aspose.cells.gridweb.data/pivottables/clear/)() | Entfernt alle PivotTable-Objekte und alle PivotCache-Objekte in der Steuerung. |
| [Contains](../../aspose.cells.gridweb.data/pivottables/contains/)(string) | Gibt true zurück, wenn ein PivotTable-Name tableName existiert. |
| [CopyTo](../../aspose.cells.gridweb.data/pivottables/copyto/)(Array, int) | Kopiert die gesamte PivotTable in ein kompatibles eindimensionales Array, beginnend beim angegebenen Index des Zielarrays |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivottables/getenumerator/)() | Gibt einen IEnumerator für die PivotTables zurück. |
| [Refresh](../../aspose.cells.gridweb.data/pivottables/refresh/)(PivotTable) | Bindet die Datenquelle erneut an den PivotTable-Bericht. |
| [RefreshAll](../../aspose.cells.gridweb.data/pivottables/refreshall/)() | Bindet die Datenquelle erneut an alle PivotTable-Berichte. |
| [Remove](../../aspose.cells.gridweb.data/pivottables/remove/)(PivotTable) | Entfernt das angegebene PivotTable-Objekt aus den PivotTables und den zugehörigen PivotCache, falls es von keiner anderen PivotTable verwendet wird |
| [RemoveAt](../../aspose.cells.gridweb.data/pivottables/removeat/)(int) | Entfernt das angegebene PivotTable-Objekt aus den PivotTables und den zugehörigen PivotCache, falls es von keiner anderen PivotTable verwendet wird |

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Bitte verwenden Sie stattdessen GridPivotTableCollection. Diese Klasse wird nach 6 Monaten seit August 2014 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

### Beispiele

```csharp

 [C#]

 //Unter der Annahme, dass das Arbeitsblatt "Sheet1" Daten enthält, wird dann ein PivotTable-Bericht darauf basierend erstellt.
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

 //Erstellt einen PivotTable-Bericht aus DataView oder DataTable.
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

### Siehe auch

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


