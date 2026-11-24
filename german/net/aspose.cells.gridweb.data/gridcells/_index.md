---
title: "Klasse GridCells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.GridWeb.Data.GridCells Klasse. Kapselt eine Sammlung von GridCell-Objekten"
type: docs
url: /de/net/aspose.cells.gridweb.data/gridcells/
---
## GridCells class

Kapselt eine Sammlung von [`GridCell`](../gridcell/) Objekten.

```csharp
public class GridCells : IEnumerable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Columns](../../aspose.cells.gridweb.data/gridcells/columns/) { get; } | Liefert die Sammlung von [`GridColumn`](../gridcolumn/) Objekten, die die einzelnen Spalten in diesem Arbeitsblatt darstellen. |
| [Count](../../aspose.cells.gridweb.data/gridcells/count/) { get; } | Liest die Anzahl der Zellen. |
| [FirstCell](../../aspose.cells.gridweb.data/gridcells/firstcell/) { get; } | Ruft die erste Zelle in diesem Arbeitsblatt ab. |
| [Item](../../aspose.cells.gridweb.data/gridcells/item/) { get; } | Liest das [`GridCell`](../gridcell/) Element am angegebenen Zeilen- und Spaltenindex der Zelle. (2 Indexer) |
| [LastCell](../../aspose.cells.gridweb.data/gridcells/lastcell/) { get; } | Ruft die letzte Zelle in diesem Arbeitsblatt ab. |
| [MaxColumn](../../aspose.cells.gridweb.data/gridcells/maxcolumn/) { get; } | Maximaler Spaltenindex der Zelle, die Daten oder Stil enthält. |
| [MaxDataColumn](../../aspose.cells.gridweb.data/gridcells/maxdatacolumn/) { get; } | Maximaler Spaltenindex der Zelle, die Daten enthält. |
| [MaxDataRow](../../aspose.cells.gridweb.data/gridcells/maxdatarow/) { get; } | Maximaler Zeilenindex der Zelle, die Daten enthält. |
| [MaxRow](../../aspose.cells.gridweb.data/gridcells/maxrow/) { get; } | Maximaler Zeilenindex der Zelle, die Daten oder einen Stil enthält. |
| [MergedCells](../../aspose.cells.gridweb.data/gridcells/mergedcells/) { get; } | Liest die Sammlung zusammengeführter Zellen. |
| [MinColumn](../../aspose.cells.gridweb.data/gridcells/mincolumn/) { get; } | Minimaler Spaltenindex jener Zellen, die in der Sammlung instanziiert wurden (schließt die Spalte, für die ein Stil für die gesamte Spalte definiert ist, aber in der keine Zelle instanziiert wurde, nicht ein). |
| [MinDataColumn](../../aspose.cells.gridweb.data/gridcells/mindatacolumn/) { get; } | Minimaler Spaltenindex der Zelle, die Daten enthält. |
| [MinDataRow](../../aspose.cells.gridweb.data/gridcells/mindatarow/) { get; } | Minimaler Zeilenindex der Zelle, die Daten enthält. |
| [MinRow](../../aspose.cells.gridweb.data/gridcells/minrow/) { get; } | Minimaler Zeilenindex der Zelle, die Daten oder einen Stil enthält. |
| [RowEnumerator](../../aspose.cells.gridweb.data/gridcells/rowenumerator/) { get; } | Gibt den Zeilen-Enumerator zurück |
| [Rows](../../aspose.cells.gridweb.data/gridcells/rows/) { get; } | Liest die Sammlung von [`GridRow`](../gridrow/) Objekten, die die einzelnen Zeilen in diesem Arbeitsblatt darstellen. |
| [StandardHeight](../../aspose.cells.gridweb.data/gridcells/standardheight/) { get; set; } | Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Punkten. |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridcells/standardheightpixels/) { get; set; } | Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Pixeln. |
| [StandardWidth](../../aspose.cells.gridweb.data/gridcells/standardwidth/) { get; set; } | Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Zeichen. |
| [StandardWidthInch](../../aspose.cells.gridweb.data/gridcells/standardwidthinch/) { get; set; } | Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Zoll. |
| [StandardWidthPixels](../../aspose.cells.gridweb.data/gridcells/standardwidthpixels/) { get; set; } | Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Pixel. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CheckCell](../../aspose.cells.gridweb.data/gridcells/checkcell/)(int, int) | Liest das [`GridCell`](../gridcell/) Element oder null am angegebenen Zeilen- und Spaltenindex der Zelle. |
| [CheckColumn](../../aspose.cells.gridweb.data/gridcells/checkcolumn/)(int) | Liefert das [`GridColumn`](../gridcolumn/) Element oder null am angegebenen Spaltenindex. |
| [CheckRow](../../aspose.cells.gridweb.data/gridcells/checkrow/)(int) | Liest das [`GridRow`](../gridrow/) Element oder null am angegebenen Zeilenindex der Zelle. |
| [Clear](../../aspose.cells.gridweb.data/gridcells/clear/)() | Löscht alle Zellen in der Sammlung. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | Löscht den Inhalt eines Bereichs. |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | Löscht den Inhalt eines Bereichs. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats)(GridCellArea) | Löscht die Formatierung eines Bereichs. |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | Löscht die Formatierung eines Bereichs. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange)(GridCellArea) | Löscht Inhalt und Formatierung eines Bereichs. |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | Löscht Inhalt und Formatierung eines Bereichs. |
| [CopyColumn](../../aspose.cells.gridweb.data/gridcells/copycolumn/)(GridCells, int, int) | Kopiert Daten und Formatierungen einer gesamten Spalte. |
| [CopyColumns](../../aspose.cells.gridweb.data/gridcells/copycolumns/)(GridCells, int, int, int) | Kopiert Daten und Formatierungen einer gesamten Spalte. |
| [CopyRow](../../aspose.cells.gridweb.data/gridcells/copyrow/)(GridCells, int, int) | Kopiert Daten und Formatierungen einer gesamten Zeile. |
| [CopyRows](../../aspose.cells.gridweb.data/gridcells/copyrows/)(GridCells, int, int, int) | Kopiert Daten und Formatierungen einiger ganzer Zeilen. |
| [DeleteBlankColumns](../../aspose.cells.gridweb.data/gridcells/deleteblankcolumns/)() | Löscht alle leeren Spalten, die keine Daten enthalten. |
| [DeleteBlankRows](../../aspose.cells.gridweb.data/gridcells/deleteblankrows/)() | Löscht alle leeren Zeilen, die keine Daten enthalten. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn)(int) | Löscht eine Spalte. |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | Löscht eine Spalte. |
| [DeleteColumns](../../aspose.cells.gridweb.data/gridcells/deletecolumns/)(int, int, bool) | Löscht mehrere Spalten. |
| [DeleteRange](../../aspose.cells.gridweb.data/gridcells/deleterange/)(int, int, int, int, GridShiftType) | Löscht einen Zellbereich und verschiebt Zellen gemäß der Verschiebungsoption. |
| [DeleteRow](../../aspose.cells.gridweb.data/gridcells/deleterow/)(int) | Löscht eine Zeile. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows)(int, int) | Löscht mehrere Zeilen. |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | Löscht mehrere Zeilen im Arbeitsblatt. |
| [Export](../../aspose.cells.gridweb.data/gridcells/export/)(int, int, int, int, bool, bool) | Exportiert Daten aus der Cells-Sammlung eines WebWorksheet in ein neues DataTable-Objekt. |
| [ExportArray](../../aspose.cells.gridweb.data/gridcells/exportarray/)(int, int, int, int) | Exportiert Daten aus der `GridCells`-Sammlung in ein zweidimensionales Array-Objekt. |
| [GetCell](../../aspose.cells.gridweb.data/gridcells/getcell/)(int, int) | Liefert das [`GridCell`](../gridcell/) Element am angegebenen Zeilen- und Spaltenindex. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/gridcells/getcolumnwidth/)(int) | Liest die Breite der angegebenen Spalte |
| [GetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthinch/)(int) | Liest die Breite der angegebenen Spalte, in Zoll. |
| [GetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthpixel/)(int) | Ermittelt die Breite der angegebenen Spalte in Pixeln. |
| [GetEnumerator](../../aspose.cells.gridweb.data/gridcells/getenumerator/)() | Gibt den Zeilen-Enumerator zurück |
| [GetRow](../../aspose.cells.gridweb.data/gridcells/getrow/)(int) | Ruft das [`GridRow`](../gridrow/)‑Element oder den angegebenen Zeilenindex der Zelle ab. |
| [GetRowHeight](../../aspose.cells.gridweb.data/gridcells/getrowheight/)(int) | Gibt die Höhe einer angegebenen Zeile zurück. |
| [GetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/getrowheightinch/)(int) | Gibt die Höhe einer angegebenen Zeile in Zoll zurück. |
| [GetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/getrowheightpixel/)(int) | Gibt die Höhe einer angegebenen Zeile in Pixel zurück. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/getrowoutlinelevel/)(int) | Liefert die Gliederungsebene der Zeile. |
| [GetViewColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getviewcolumnwidthpixel/)(int) | Erhalte die Breite in verschiedenen Ansichtstypen. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns)(int, int) | Gruppiert Spalten. |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | Gruppiert Spalten. |
| [GroupRows](../../aspose.cells.gridweb.data/gridcells/grouprows/)(int, int) | Gruppiert Zeilen. |
| [HideColumn](../../aspose.cells.gridweb.data/gridcells/hidecolumn/)(int) | Blendet eine Spalte aus. |
| [HideRow](../../aspose.cells.gridweb.data/gridcells/hiderow/)(int) | Blendet eine Zeile aus. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn)(int) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns)(int, int) | Fügt mehrere Spalten in das Arbeitsblatt ein. |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | Fügt mehrere Spalten in das Arbeitsblatt ein. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange)(GridCellArea, GridShiftType) | Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption. |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange/#insertrange_1)(GridCellArea, int, GridShiftType, bool) | Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption. |
| [InsertRow](../../aspose.cells.gridweb.data/gridcells/insertrow/)(int) | Fügt eine neue Zeile in das Arbeitsblatt ein. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows)(int, int) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [IsBlankColumn](../../aspose.cells.gridweb.data/gridcells/isblankcolumn/)(int) | Prüft, ob die angegebene Spalte leer ist (enthält keine Daten). |
| [IsColumnHidden](../../aspose.cells.gridweb.data/gridcells/iscolumnhidden/)(int) | Überprüft, ob eine Spalte am angegebenen Index ausgeblendet ist. |
| [IsRowHidden](../../aspose.cells.gridweb.data/gridcells/isrowhidden/)(int) | Überprüft, ob eine Zeile am angegebenen Index ausgeblendet ist. |
| [Merge](../../aspose.cells.gridweb.data/gridcells/merge/)(int, int, int, int) | Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen. |
| [MoveRange](../../aspose.cells.gridweb.data/gridcells/moverange/)(GridCellArea, int, int) | Verschiebt den Bereich. |
| [RemoveDuplicates](../../aspose.cells.gridweb.data/gridcells/removeduplicates/)(int, int, int, int) | Entfernt doppelte Werte im Bereich. |
| [RemoveFormulas](../../aspose.cells.gridweb.data/gridcells/removeformulas/)() | Entfernt alle Formeln und ersetzt sie durch den Wert der Formel. |
| [SetBorders](../../aspose.cells.gridweb.data/gridcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Setzt Rahmen für einen Zellenbereich. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/gridcells/setcolumnwidth/)(int, double) | Setzt die Breite der angegebenen Spalte. |
| [SetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthinch/)(int, double) | Setzt die Spaltenbreite in Zoll. |
| [SetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthpixel/)(int, int) | Setzt die Spaltenbreite in Pixeln. |
| [SetRowHeight](../../aspose.cells.gridweb.data/gridcells/setrowheight/)(int, double) | Setzt die Höhe der angegebenen Zeile. |
| [SetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/setrowheightinch/)(int, double) | Setzt die Zeilenhöhe in Zoll. |
| [SetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/setrowheightpixel/)(int, int) | Setzt die Zeilenhöhe in Pixeln. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/setrowoutlinelevel/)(int, int) | Setzt die Gliederungsebene der Zeile. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle_1)(string, GridTableItemStyle) | Setzt den Stil für einen angegebenen Zellbereich. |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle/#setstyle)(int, int, int, int, GridTableItemStyle) | Setzt den Stil für einen angegebenen Zellbereich. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | Sortiert die Daten aufsteigend/absteigend von oben nach unten in einem Bereich eines Arbeitsblatts nach angegebenem Spaltenindex. Sortiert die Daten aufsteigend/absteigend von links nach rechts in einem Bereich eines Arbeitsblatts nach angegebenem Zeilenindex. |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | Sortiert die Daten aufsteigend/absteigend von oben nach unten in einem Bereich eines Arbeitsblatts nach angegebenem Spaltenindex. Sortiert die Daten aufsteigend/absteigend von links nach rechts in einem Bereich eines Arbeitsblatts nach angegebenem Zeilenindex. |
| [UngroupColumns](../../aspose.cells.gridweb.data/gridcells/ungroupcolumns/)(int, int) | Löst die Gruppierung von Spalten auf. |
| [UngroupRows](../../aspose.cells.gridweb.data/gridcells/ungrouprows/)(int, int) | Löst die Gruppierung von Zeilen auf. |
| [UnhideColumn](../../aspose.cells.gridweb.data/gridcells/unhidecolumn/)(int, double) | Blendet eine Spalte ein |
| [UnhideRow](../../aspose.cells.gridweb.data/gridcells/unhiderow/)(int) | Blendet eine Zeile ein. |
| [UnMerge](../../aspose.cells.gridweb.data/gridcells/unmerge/)(int, int, int, int) | Löst einen angegebenen Bereich zusammengeführter Zellen auf. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/gridcells/cellindextoname/)(int, int) | Ermittelt den Zellnamen anhand seiner Zeilen- und Spaltenindizes. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/gridcells/cellnametoindex/)(string, out int, out int) | Ermittelt die Zeilen‑ und Spaltenindizes der Zelle anhand ihres Namens |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/gridcells/columnindextoname/)(int) | Ermittelt den Spaltennamen anhand des Spaltenindex. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/gridcells/columnnametoindex/)(string) | Ermittelt den Spaltenindex anhand des Spaltennamens. |

### Siehe auch

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


