---
title: "Klasse GridCells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridDesktop.Data.GridCells Klasse. Kapselt eine Sammlung von Cell-Objekten."
type: docs
url: /de/net/aspose.cells.griddesktop.data/gridcells/
---
## GridCells class

Kapselt eine Sammlung von Cell-Objekten.

```csharp
public class GridCells : IEnumerable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Columns](../../aspose.cells.griddesktop.data/gridcells/columns/) { get; } |  |
| [Count](../../aspose.cells.griddesktop.data/gridcells/count/) { get; } | Liest die Anzahl der Zellen. |
| [FirstCell](../../aspose.cells.griddesktop.data/gridcells/firstcell/) { get; } | Ruft die erste Zelle in diesem Arbeitsblatt ab. |
| [Item](../../aspose.cells.griddesktop.data/gridcells/item/) { get; } | Liest das [`GridCell`](../gridcell/) Element am angegebenen Zeilen- und Spaltenindex der Zelle. (2 Indexer) |
| [LastCell](../../aspose.cells.griddesktop.data/gridcells/lastcell/) { get; } | Ruft die letzte Zelle in diesem Arbeitsblatt ab. |
| [MaxColumn](../../aspose.cells.griddesktop.data/gridcells/maxcolumn/) { get; } | Maximaler Spaltenindex der Zelle, die Daten oder Stil enthält. |
| [MaxDataColumn](../../aspose.cells.griddesktop.data/gridcells/maxdatacolumn/) { get; } | Maximaler Spaltenindex der Zelle, die Daten enthält. |
| [MaxDataRow](../../aspose.cells.griddesktop.data/gridcells/maxdatarow/) { get; } | Maximaler Zeilenindex der Zelle, die Daten enthält. |
| [MaxRow](../../aspose.cells.griddesktop.data/gridcells/maxrow/) { get; } | Maximaler Zeilenindex der Zelle, die Daten oder einen Stil enthält. |
| [MergedCells](../../aspose.cells.griddesktop.data/gridcells/mergedcells/) { get; } | Liest die Sammlung zusammengeführter Zellen. |
| [MinColumn](../../aspose.cells.griddesktop.data/gridcells/mincolumn/) { get; } | Minimaler Spaltenindex jener Zellen, die in der Sammlung instanziiert wurden (schließt die Spalte, für die ein Stil für die gesamte Spalte definiert ist, aber in der keine Zelle instanziiert wurde, nicht ein). |
| [MinDataColumn](../../aspose.cells.griddesktop.data/gridcells/mindatacolumn/) { get; } | Minimaler Spaltenindex der Zelle, die Daten enthält. |
| [MinDataRow](../../aspose.cells.griddesktop.data/gridcells/mindatarow/) { get; } | Minimaler Zeilenindex der Zelle, die Daten enthält. |
| [MinRow](../../aspose.cells.griddesktop.data/gridcells/minrow/) { get; } | Minimaler Zeilenindex der Zelle, die Daten oder einen Stil enthält. |
| [RowEnumerator](../../aspose.cells.griddesktop.data/gridcells/rowenumerator/) { get; } | Gibt den Zeilen-Enumerator zurück |
| [Rows](../../aspose.cells.griddesktop.data/gridcells/rows/) { get; } | Liest die Sammlung von [`GridRow`](../gridrow/) Objekten, die die einzelnen Zeilen in diesem Arbeitsblatt darstellen. |
| [StandardHeight](../../aspose.cells.griddesktop.data/gridcells/standardheight/) { get; set; } | Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Punkten. |
| [StandardHeightPixels](../../aspose.cells.griddesktop.data/gridcells/standardheightpixels/) { get; set; } | Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Pixeln. |
| [StandardWidth](../../aspose.cells.griddesktop.data/gridcells/standardwidth/) { get; set; } | Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Zeichen. |
| [StandardWidthInch](../../aspose.cells.griddesktop.data/gridcells/standardwidthinch/) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.griddesktop.data/gridcells/standardwidthpixels/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CheckCell](../../aspose.cells.griddesktop.data/gridcells/checkcell/)(int, int) | Liest das [`GridCell`](../gridcell/) Element oder null am angegebenen Zeilen- und Spaltenindex der Zelle. |
| [CheckRow](../../aspose.cells.griddesktop.data/gridcells/checkrow/)(int) | Liest das [`GridRow`](../gridrow/) Element oder null am angegebenen Zeilenindex der Zelle. |
| [Clear](../../aspose.cells.griddesktop.data/gridcells/clear/)() | Löscht alle Zellen in der Sammlung. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | Löscht den Inhalt eines Bereichs. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | Löscht den Inhalt eines Bereichs. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats)(GridCellArea) | Löscht die Formatierung eines Bereichs. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | Löscht die Formatierung eines Bereichs. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange)(GridCellArea) | Löscht Inhalt und Formatierung eines Bereichs. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | Löscht Inhalt und Formatierung eines Bereichs. |
| [CopyColumn](../../aspose.cells.griddesktop.data/gridcells/copycolumn/)(GridCells, int, int) | Kopiert Daten und Formatierungen einer gesamten Spalte. |
| [CopyColumns](../../aspose.cells.griddesktop.data/gridcells/copycolumns/)(GridCells, int, int, int) | Kopiert Daten und Formatierungen einer gesamten Spalte. |
| [CopyRow](../../aspose.cells.griddesktop.data/gridcells/copyrow/)(GridCells, int, int) | Kopiert Daten und Formatierungen einer gesamten Zeile. |
| [CopyRows](../../aspose.cells.griddesktop.data/gridcells/copyrows/)(GridCells, int, int, int) | Kopiert Daten und Formatierungen einiger ganzer Zeilen. |
| [DeleteBlankColumns](../../aspose.cells.griddesktop.data/gridcells/deleteblankcolumns/)() | Löscht alle leeren Spalten, die keine Daten enthalten. |
| [DeleteBlankRows](../../aspose.cells.griddesktop.data/gridcells/deleteblankrows/)() | Löscht alle leeren Zeilen, die keine Daten enthalten. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn)(int) | Löscht eine Spalte. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | Löscht eine Spalte. |
| [DeleteColumns](../../aspose.cells.griddesktop.data/gridcells/deletecolumns/)(int, int, bool) | Löscht mehrere Spalten. |
| [DeleteRow](../../aspose.cells.griddesktop.data/gridcells/deleterow/)(int) | Löscht eine Zeile. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows)(int, int) | Löscht mehrere Zeilen. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | Löscht mehrere Zeilen im Arbeitsblatt. |
| [GetCellStyle](../../aspose.cells.griddesktop.data/gridcells/getcellstyle/)(int, int) | Ermittelt den Stil der angegebenen Zelle. |
| [GetColumn](../../aspose.cells.griddesktop.data/gridcells/getcolumn/)(int) | Liest das [`GridColumn`](../gridcolumn/) Element am angegebenen Spaltenindex der Zelle. |
| [GetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidth/)(int) | Liest die Breite der angegebenen Spalte |
| [GetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthinch/)(int) | Liest die Breite der angegebenen Spalte, in Zoll. |
| [GetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthpixel/)(int) | Ermittelt die Breite der angegebenen Spalte in Pixeln. |
| [GetEnumerator](../../aspose.cells.griddesktop.data/gridcells/getenumerator/)() | Gibt den Zeilen-Enumerator zurück |
| [GetRow](../../aspose.cells.griddesktop.data/gridcells/getrow/)(int) | Ruft das [`GridRow`](../gridrow/)‑Element oder den angegebenen Zeilenindex der Zelle ab. |
| [GetRowHeight](../../aspose.cells.griddesktop.data/gridcells/getrowheight/)(int) | Gibt die Höhe einer angegebenen Zeile zurück. |
| [GetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/getrowheightinch/)(int) | Gibt die Höhe einer angegebenen Zeile in Zoll zurück. |
| [GetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/getrowheightpixel/)(int) | Gibt die Höhe einer angegebenen Zeile in Pixel zurück. |
| [GetViewColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getviewcolumnwidthpixel/)(int) | Erhalte die Breite in verschiedenen Ansichtstypen. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns)(int, int) | Gruppiert Spalten. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | Gruppiert Spalten. |
| [GroupRows](../../aspose.cells.griddesktop.data/gridcells/grouprows/)(int, int) | Gruppiert Zeilen. |
| [HideColumn](../../aspose.cells.griddesktop.data/gridcells/hidecolumn/)(int) | Blendet eine Spalte aus. |
| [HideColumns](../../aspose.cells.griddesktop.data/gridcells/hidecolumns/)(int, int) | Blendet mehrere Spalten aus. |
| [HideRow](../../aspose.cells.griddesktop.data/gridcells/hiderow/)(int) | Blendet eine Zeile aus. |
| [HideRows](../../aspose.cells.griddesktop.data/gridcells/hiderows/)(int, int) | Blendet mehrere Zeilen aus. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn)(int) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns)(int, int) | Fügt mehrere Spalten in das Arbeitsblatt ein. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | Fügt mehrere Spalten in das Arbeitsblatt ein. |
| [InsertRow](../../aspose.cells.griddesktop.data/gridcells/insertrow/)(int) | Fügt eine neue Zeile in das Arbeitsblatt ein. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows)(int, int) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [IsBlankColumn](../../aspose.cells.griddesktop.data/gridcells/isblankcolumn/)(int) | Prüft, ob die angegebene Spalte leer ist (enthält keine Daten). |
| [IsColumnHidden](../../aspose.cells.griddesktop.data/gridcells/iscolumnhidden/)(int) | Überprüft, ob eine Spalte am angegebenen Index ausgeblendet ist. |
| [IsRowHidden](../../aspose.cells.griddesktop.data/gridcells/isrowhidden/)(int) | Überprüft, ob eine Zeile am angegebenen Index ausgeblendet ist. |
| [Merge](../../aspose.cells.griddesktop.data/gridcells/merge/)(int, int, int, int) | Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen. |
| [RemoveFormulas](../../aspose.cells.griddesktop.data/gridcells/removeformulas/)() | Entfernt alle Formeln und ersetzt sie durch den Wert der Formel. |
| [SetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidth/)(int, double) | Setzt die Breite der angegebenen Spalte. |
| [SetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthinch/)(int, double) | Setzt die Spaltenbreite in Zoll. |
| [SetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthpixel/)(int, int) | Setzt die Spaltenbreite in Pixeln. |
| [SetRowHeight](../../aspose.cells.griddesktop.data/gridcells/setrowheight/)(int, double) | Setzt die Höhe der angegebenen Zeile. |
| [SetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/setrowheightinch/)(int, double) | Setzt die Zeilenhöhe in Zoll. |
| [SetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/setrowheightpixel/)(int, int) | Setzt die Zeilenhöhe in Pixeln. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle)(CellRange, Style) | Setzt den Stil für einen angegebenen Zellbereich. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_2)(string, Style) | Setzt den Stil für einen angegebenen Zellbereich. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_1)(int, int, int, int, Style) | Setzt den Stil für einen angegebenen Zellbereich. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | Sortiert die Daten aufsteigend/absteigend von oben nach unten in einem Bereich eines Arbeitsblatts nach angegebenem Spaltenindex. Sortiert die Daten aufsteigend/absteigend von links nach rechts in einem Bereich eines Arbeitsblatts nach angegebenem Zeilenindex. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) | Sortiert die Daten des Bereichs. |
| [SortAsNumber](../../aspose.cells.griddesktop.data/gridcells/sortasnumber/)(int, int, int, int, int[], SortOrder[], SortOrientation) | Sortiert die Daten des Bereichs (die Schlüsselspaltendaten müssen numerisch sein). |
| [UngroupColumns](../../aspose.cells.griddesktop.data/gridcells/ungroupcolumns/)(int, int) | Löst die Gruppierung von Spalten auf. |
| [UngroupRows](../../aspose.cells.griddesktop.data/gridcells/ungrouprows/)(int, int) | Löst die Gruppierung von Zeilen auf. |
| [UnhideColumn](../../aspose.cells.griddesktop.data/gridcells/unhidecolumn/)(int, double) | Blendet eine Spalte ein |
| [UnhideColumns](../../aspose.cells.griddesktop.data/gridcells/unhidecolumns/)(int, int, double) | Blendet mehrere Spalten ein. |
| [UnhideRow](../../aspose.cells.griddesktop.data/gridcells/unhiderow/)(int, int) | Blendet eine Zeile ein. |
| [UnhideRows](../../aspose.cells.griddesktop.data/gridcells/unhiderows/)(int, int, double) | Blendet die ausgeblendeten Zeilen ein. |
| [UnMerge](../../aspose.cells.griddesktop.data/gridcells/unmerge/)(int, int, int, int) | Löst einen angegebenen Bereich zusammengeführter Zellen auf. |
| static [CellIndexToName](../../aspose.cells.griddesktop.data/gridcells/cellindextoname/)(int, int) | Ermittelt den Zellnamen anhand seiner Zeilen- und Spaltenindizes. |
| static [CellNameToIndex](../../aspose.cells.griddesktop.data/gridcells/cellnametoindex/)(string, out int, out int) | Ermittelt die Zeilen‑ und Spaltenindizes der Zelle anhand ihres Namens |
| static [ColumnIndexToName](../../aspose.cells.griddesktop.data/gridcells/columnindextoname/)(int) | Ermittelt den Spaltennamen anhand des Spaltenindex. |
| static [ColumnNameToIndex](../../aspose.cells.griddesktop.data/gridcells/columnnametoindex/)(string) | Ermittelt den Spaltenindex anhand des Spaltennamens. |

### Siehe auch

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


