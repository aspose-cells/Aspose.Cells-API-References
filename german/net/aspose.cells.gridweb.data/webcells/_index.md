---
title: "Klasse WebCells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.WebCells Klasse."
type: docs
url: /de/net/aspose.cells.gridweb.data/webcells/
---
## WebCells class

```csharp
[Obsolete("This class is obsolete; use  GridCells instead")]
public class WebCells
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/webcells/count/) { get; } | Liest die Anzahl der Zellen. |
| [Item](../../aspose.cells.gridweb.data/webcells/item/) { get; } | Ruft das Cell-Element am angegebenen Zeilenindex und Spaltenindex ab. (2 Indexer) |
| [MaxColumn](../../aspose.cells.gridweb.data/webcells/maxcolumn/) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/webcells/maxrow/) { get; } |  |
| [MergedCells](../../aspose.cells.gridweb.data/webcells/mergedcells/) { get; } | Liest die Sammlung zusammengeführter Zellen. |
| [MinColumn](../../aspose.cells.gridweb.data/webcells/mincolumn/) { get; } | Minimale Spaltennummer der Zelle, die Daten oder Stil enthält. |
| [MinRow](../../aspose.cells.gridweb.data/webcells/minrow/) { get; } | Minimale Zeilennummer der Zelle, die Daten oder Stil enthält. |
| [StandardHeight](../../aspose.cells.gridweb.data/webcells/standardheight/) { get; set; } | Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Punkten. |
| [StandardWidth](../../aspose.cells.gridweb.data/webcells/standardwidth/) { get; set; } | Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Zeichen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/webcells/clear/)() |  |
| [ClearContents](../../aspose.cells.gridweb.data/webcells/clearcontents/)(int, int, int, int) | Löscht den Inhalt eines Bereichs. |
| [DeleteColumn](../../aspose.cells.gridweb.data/webcells/deletecolumn/)(int) | Löscht eine Spalte. |
| [DeleteRow](../../aspose.cells.gridweb.data/webcells/deleterow/)(int) | Löscht eine Zeile. |
| [DeleteRows](../../aspose.cells.gridweb.data/webcells/deleterows/)(int, int) | Löscht mehrere Zeilen. Diese Methode ist beim Batch-Löschen von Zeilen viel schneller als DeleteRow. |
| [Export](../../aspose.cells.gridweb.data/webcells/export/)(int, int, int, int, bool, bool) | Exportiert Daten aus der Cells-Sammlung eines WebWorksheet in ein neues DataTable-Objekt. |
| [ExportArray](../../aspose.cells.gridweb.data/webcells/exportarray/)(int, int, int, int) | Exportiert Daten aus der Cells-Sammlung in ein zweidimensionales Array-Objekt. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/webcells/getcolumncaption/)(int) | Liefert die Spaltenbeschriftung. Wenn die Beschriftung nicht gesetzt ist, wird ein leerer String zurückgegeben. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/webcells/getcolumnreadonly/)(int) | Ermittelt, ob eine Spalte schreibgeschützt ist. Dies ist eine erweiterte Methode von GridWeb speziell, sie wird in der tatsächlichen Excel-Datei nicht beibehalten und wirkt sich nicht aus. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/webcells/getcolumnwidth/)(int) | Liest die Breite der angegebenen Spalte |
| [GetEnumerator](../../aspose.cells.gridweb.data/webcells/getenumerator/)() | Gibt den Zellen-Enumerator zurück |
| [GetRowCaption](../../aspose.cells.gridweb.data/webcells/getrowcaption/)(int) | Liefert die Zeilenbeschriftung. Wenn die Beschriftung nicht gesetzt ist, wird eine leere Zeichenkette zurückgegeben. |
| [GetRowHeight](../../aspose.cells.gridweb.data/webcells/getrowheight/)(int) | Gibt die Höhe einer angegebenen Zeile zurück. |
| [GetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/getrowhiddenstatus/)(int) | Ermittelt den ausgeblendeten Status einer angegebenen Zeile. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/getrowoutlinelevel/)(int) | Liefert die Gliederungsebene der Zeile. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/webcells/getrowreadonly/)(int) | Ermittelt, ob eine Zeile schreibgeschützt ist. Dies ist eine erweiterte Methode von GridWeb speziell, sie wird in der tatsächlichen Excel-Datei nicht beibehalten und wirkt sich nicht aus. |
| [InsertColumn](../../aspose.cells.gridweb.data/webcells/insertcolumn/)(int) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [InsertRow](../../aspose.cells.gridweb.data/webcells/insertrow/)(int) | Fügt eine neue Zeile in das Arbeitsblatt ein. |
| [InsertRows](../../aspose.cells.gridweb.data/webcells/insertrows/)(int, int) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [Merge](../../aspose.cells.gridweb.data/webcells/merge/)(int, int, int, int) |  |
| [SetBorders](../../aspose.cells.gridweb.data/webcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Setzt Rahmen für einen Zellenbereich. |
| [SetColumnCaption](../../aspose.cells.gridweb.data/webcells/setcolumncaption/)(int, string) | Setzt die Beschriftung für die Spalte. Bitte beachten Sie, dass dies ein erweitertes Attribut ist und nicht in der Excel-Datei beibehalten werden kann. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/webcells/setcolumnreadonly/)(int, bool) | Setzt eine Spalte auf schreibgeschützt, sodass der Benutzer sie nicht von der Clientseite löschen kann. Dies ist eine erweiterte Methode von GridWeb speziell, sie wird in der tatsächlichen Excel-Datei nicht beibehalten und wirkt sich nicht aus. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/webcells/setcolumnwidth/)(int, Unit) | Setzt die Breite der angegebenen Spalte. Der akzeptierte Breitentyp ist Punkt, Pixel oder Zoll. |
| [SetRowCaption](../../aspose.cells.gridweb.data/webcells/setrowcaption/)(int, string) | Setzt die Beschriftung für die Zeile. |
| [SetRowHeight](../../aspose.cells.gridweb.data/webcells/setrowheight/)(int, Unit) | Setzt die Höhe der angegebenen Zeile. Der akzeptierte Höhentyp ist Punkt, Pixel oder Zoll. |
| [SetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/setrowhiddenstatus/)(int, bool) | Setzt den ausgeblendeten Status einer angegebenen Zeile. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevel/)(int, int) | Setzt die Gliederungsebene der Zeile. |
| [SetRowOutlineLevelAndStatus](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevelandstatus/)(int, int, bool) | Setzt die Gliederungsebene der Zeile. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/webcells/setrowreadonly/)(int, bool) | Setzt eine Zeile auf schreibgeschützt, sodass der Benutzer sie nicht von der Clientseite löschen kann. Dies ist eine erweiterte Methode von GridWeb speziell, sie wird in der tatsächlichen Excel-Datei nicht beibehalten und wirkt sich nicht aus. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle_1)(string, TableItemStyle) | Setzt den Stil für einen angegebenen Zellbereich. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle)(int, int, int, int, TableItemStyle) | Setzt den Stil für einen angegebenen Zellbereich. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort)(int, int, int, int, int) | Sortiert die Daten aufsteigend von oben nach unten in einem Bereich eines WebWorksheet nach angegebenem Spaltenindex. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_2)(int, int, int, int, int[]) | Sortiert die Daten aufsteigend von oben nach unten in einem Bereich eines WebWorksheet nach Feldern, die durch ein Array von Spaltenindizes angegeben sind. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_1)(int, int, int, int, int, SortByOrder, SortOrientation, bool) | Sortiert die Daten aufsteigend von oben nach unten in einem Bereich eines WebWorksheet nach angegebenem Spaltenindex. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_3)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | Sortiert die Daten aufsteigend in einem Bereich eines WebWorksheet nach Feldern, die durch ein Index-Array angegeben sind. |
| [UnMerge](../../aspose.cells.gridweb.data/webcells/unmerge/)(int, int, int, int) | Löst einen angegebenen Bereich zusammengeführter Zellen auf. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/webcells/cellindextoname/)(int, int) | Ermittelt den Zellnamen anhand seiner Zeilen- und Spaltenindizes. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/webcells/cellnametoindex/)(string, out int, out int) | Ermittelt die Zeilen‑ und Spaltenindizes der Zelle anhand ihres Namens |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/webcells/columnindextoname/)(int) | Ermittelt den Spaltennamen anhand des Spaltenindex. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/webcells/columnnametoindex/)(string) | Ermittelt den Spaltenindex anhand des Spaltennamens. |

### Hinweise

HINWEIS: Diese Klasse ist jetzt veraltet. Bitte verwenden Sie stattdessen GridCells. Diese Klasse wird nach 6 Monaten seit August 2014 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

### Siehe auch

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


