---
title: "Klasse PivotCaches"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.PivotCaches Klasse. Stellt die Sammlung von Speicher‑Caches aus den PivotTable-Berichten in einer Arbeitsmappe dar. Jeder Speicher‑Cache wird durch ein PivotCache‑Objekt repräsentiert."
type: docs
url: /de/net/aspose.cells.gridweb.data/pivotcaches/
---
## PivotCaches class

Stellt die Sammlung von Speicher‑Caches aus den PivotTable-Berichten in einer Arbeitsmappe dar. Jeder Speicher‑Cache wird durch ein [`PivotCache`](../pivotcache/) Objekt repräsentiert.

```csharp
[Obsolete("This class is obsolete; use GridPivotTableCollection instead")]
public class PivotCaches : ICollection
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/pivotcaches/count/) { get; } | Gibt die Anzahl der in der PivotCaches-Instanz enthaltenen Elemente zurück. |
| [IsSynchronized](../../aspose.cells.gridweb.data/pivotcaches/issynchronized/) { get; } | Gibt einen Wert zurück, der angibt, ob der Zugriff auf die PivotCaches synchronisiert (thread‑sicher) ist. |
| [Item](../../aspose.cells.gridweb.data/pivotcaches/item/) { get; } | Gibt das PivotCache-Objekt nach Index zurück. (2 Indexer) |
| [Parent](../../aspose.cells.gridweb.data/pivotcaches/parent/) { get; } | Liefert das übergeordnete Objekt für das angegebene Objekt. Nur lesbar. |
| [SyncRoot](../../aspose.cells.gridweb.data/pivotcaches/syncroot/) { get; } | Liefert ein Objekt, das verwendet werden kann, um den Zugriff auf die PivotCaches zu synchronisieren. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_2)(DataTable) | Fügt einen PivotCache aus einer DataTable hinzu. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_4)(DataView) | Fügt einen PivotCache aus einer DataView hinzu. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_3)(DataTable, string) | Fügt einen PivotCahe aus einer DataTable mit dem angegebenen Namen hinzu. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_5)(DataView, string) | Fügt einen PivotCahe aus einer DataView mit dem angegebenen Namen hinzu. |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add)(WebWorksheet, WebCellArea) | Fügt einen PivotCache aus sheet hinzu |
| [Add](../../aspose.cells.gridweb.data/pivotcaches/add/#add_1)(WebWorksheet, WebCellArea, string) | Fügt einen PivotCache aus sheet mit dem angegebenen Namen hinzu |
| [Clear](../../aspose.cells.gridweb.data/pivotcaches/clear/)() | Entfernt alle PivotCache-Objekte und alle PivotTable-Objekte in der Steuerung. |
| [CopyTo](../../aspose.cells.gridweb.data/pivotcaches/copyto/)(Array, int) | Kopiert den gesamten PivotCache in ein kompatibles eindimensionales Array, beginnend beim angegebenen Index des Zielarrays |
| [GetEnumerator](../../aspose.cells.gridweb.data/pivotcaches/getenumerator/)() | Gibt einen IEnumerator für die PivotCaches zurück. |
| [IndexOf](../../aspose.cells.gridweb.data/pivotcaches/indexof/)(PivotCache) | Gibt den Index des angegebenen PivotCache in der Sammlung zurück. |
| [Remove](../../aspose.cells.gridweb.data/pivotcaches/remove/)(PivotCache) | Entfernt das angegebene PivotCache-Objekt aus den PivotCaches und der zugehörigen PivotTable, wobei der pivotCache als Datenquelle verwendet wird. |
| [RemoveAt](../../aspose.cells.gridweb.data/pivotcaches/removeat/)(int) | Entfernt das angegebene PivotCache-Objekt aus den PivotCaches und der zugehörigen PivotTable, wobei der pivotCache als Datenquelle verwendet wird. |

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


