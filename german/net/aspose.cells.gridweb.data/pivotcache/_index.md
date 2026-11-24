---
title: "Klasse PivotCache"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.PivotCache class. Stellt den Speicher-Cache für einen PivotTable-Bericht dar. Das PivotCache-Objekt ist Mitglied der PivotCaches-Sammlung"
type: docs
url: /de/net/aspose.cells.gridweb.data/pivotcache/
---
## PivotCache class

Stellt den Speicher-Cache für einen PivotTable-Bericht dar. Das PivotCache-Objekt ist Mitglied der [`PivotCaches`](../pivotcaches/)‑Sammlung.

```csharp
[Obsolete("This class is obsolete; use GridPivotTable instead")]
public class PivotCache
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DataTable](../../aspose.cells.gridweb.data/pivotcache/datatable/) { get; } | Gibt die Datenquelle von System.Data.DataTable für den PivotTable-Bericht zurück. |
| [DataView](../../aspose.cells.gridweb.data/pivotcache/dataview/) { get; } | Gibt die Datenquelle von System.Data.DataView für den PivotTable-Bericht zurück. |
| [Index](../../aspose.cells.gridweb.data/pivotcache/index/) { get; } | Gibt den Index dieses Objekts im übergeordneten Element zurück |
| [Name](../../aspose.cells.gridweb.data/pivotcache/name/) { get; } | Gibt den Namen von PivotCache.Re zurück |
| [Parent](../../aspose.cells.gridweb.data/pivotcache/parent/) { get; } | Gibt das übergeordnete Objekt für das angegebene Objekt (den Container von PivotCache) zurück. Nur lesbar. |
| [SourceCellArea](../../aspose.cells.gridweb.data/pivotcache/sourcecellarea/) { get; } | Gibt den Bereich der Datenquelle zurück, der mit SourceSheet verwendet wird. |
| [SourceSheet](../../aspose.cells.gridweb.data/pivotcache/sourcesheet/) { get; } | Gibt die Datenquelle von WebWorksheet für den PivotTable-Bericht zurück. |
| [SourceType](../../aspose.cells.gridweb.data/pivotcache/sourcetype/) { get; } | Stellt den Typ der Quelldaten dar |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable)() | Erstellt einen PivotTable-Bericht in ein neues Blatt. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_3)(string) | Erstellt einen PivotTable-Bericht in ein neues Blatt. Der Name des pivotTable-Objekts |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_1)(WebWorksheet, WebCell) | Erstellt einen PivotTable-Bericht im targetSheet. |
| [CreatePivotTable](../../aspose.cells.gridweb.data/pivotcache/createpivottable/#createpivottable_2)(WebWorksheet, WebCell, string) | Erstellt einen PivotTable-Bericht im targetSheet. |
| override [Equals](../../aspose.cells.gridweb.data/pivotcache/equals/)(object) | Bestimmt, ob zwei Object-Instanzen gleich sind. |
| override [GetHashCode](../../aspose.cells.gridweb.data/pivotcache/gethashcode/)() | Dient als Hash-Funktion für einen bestimmten Typ, geeignet für den Einsatz in Hash-Algorithmen und Datenstrukturen wie einer Hashtabelle. |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_1)(DataTable) | Setzt die Quelldaten zurück |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource_2)(DataView) | Setzt die Quelldaten zurück |
| [ResetDataSource](../../aspose.cells.gridweb.data/pivotcache/resetdatasource/#resetdatasource)(WebWorksheet, WebCellArea) | Setzt die Quelldaten zurück |
| override [ToString](../../aspose.cells.gridweb.data/pivotcache/tostring/)() | Gibt einen String zurück, der das aktuelle Object darstellt |

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Bitte verwenden Sie stattdessen GridPivotTable. Diese Klasse wird nach 6 Monaten ab August 2014 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

Verwendet die PivotCache-Methode, um ein PivotCache-Objekt für einen PivotTable-Bericht zurückzugeben (jeder Bericht hat nur einen Cache). Die Quelldaten von PivotCache stammen von WebWorksheet, DataTable und so weiter.

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


