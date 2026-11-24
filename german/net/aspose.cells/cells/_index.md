---
title: "Klasse Cells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Cells‑Klasse. Kapselt eine Sammlung von zellbezogenen Objekten wie Cell, Row …usw."
type: docs
url: /de/net/aspose.cells/cells/
---
## Cells class

Kapselt eine Sammlung von zellbezogenen Objekten, wie [`Cell`](../cell/), [`Row`](../row/), …usw.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns/) { get; } | Ruft die Sammlung von [`Column`](../column/) Objekten ab, die die einzelnen Spalten in diesem Arbeitsblatt darstellt. |
| [Count](../../aspose.cells/cells/count/) { get; } | Ruft die Gesamtanzahl der instanziierten Cell‑Objekte ab. |
| [CountLarge](../../aspose.cells/cells/countlarge/) { get; } | Ruft die Gesamtanzahl der instanziierten Cell‑Objekte ab. |
| [FirstCell](../../aspose.cells/cells/firstcell/) { get; } | Ruft die erste Zelle in diesem Arbeitsblatt ab. |
| [IsDefaultColumnHidden](../../aspose.cells/cells/isdefaultcolumnhidden/) { get; set; } |  |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched/) { get; set; } | Gibt an, dass Zeilenhöhe und Standard‑Schriftgröße übereinstimmen. |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden/) { get; set; } | Gibt an, ob die Zeile standardmäßig ausgeblendet ist. |
| [Item](../../aspose.cells/cells/item/) { get; } | Ruft das [`Cell`](../cell/)‑Element am angegebenen Zeilen‑ und Spaltenindex ab. (2 Indexer) |
| [LastCell](../../aspose.cells/cells/lastcell/) { get; } | Ruft die letzte Zelle in diesem Arbeitsblatt ab. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn/) { get; } | Maximaler Spaltenindex jener Zellen, die in der Sammlung instanziiert wurden (schließt die Spalte, für die ein Stil für die gesamte Spalte definiert ist, aber in der keine Zelle instanziiert wurde, nicht ein). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn/) { get; } | Maximaler Spaltenindex der Zelle, die Daten enthält. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow/) { get; } | Maximaler Zeilenindex der Zelle, die Daten enthält. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange/) { get; } | Ruft den maximalen Bereich ab, der Daten, zusammengeführte Zellen und Formen enthält. |
| [MaxRow](../../aspose.cells/cells/maxrow/) { get; } | Maximaler Zeilenindex der Zelle, die Daten oder einen Stil enthält. |
| [MemorySetting](../../aspose.cells/cells/memorysetting/) { get; set; } | Liest oder legt die Speicherverbrauchs‑Option für diese Zellen fest. |
| [MergedCells](../../aspose.cells/cells/mergedcells/) { get; } | (**Obsolete.**) Ruft die Sammlung zusammengeführter Zellen ab. |
| [MinColumn](../../aspose.cells/cells/mincolumn/) { get; } | Minimaler Spaltenindex jener Zellen, die in der Sammlung instanziiert wurden (schließt die Spalte, für die ein Stil für die gesamte Spalte definiert ist, aber in der keine Zelle instanziiert wurde, nicht ein). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn/) { get; } | Minimaler Spaltenindex der Zelle, die Daten enthält. |
| [MinDataRow](../../aspose.cells/cells/mindatarow/) { get; } | Minimaler Zeilenindex der Zelle, die Daten enthält. |
| [MinRow](../../aspose.cells/cells/minrow/) { get; } | Minimaler Zeilenindex der Zelle, die Daten oder einen Stil enthält. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading/) { get; set; } | Liest oder legt fest, ob das Zellen‑Datenmodell Multi‑Thread‑Lesen unterstützen soll. Der Standardwert dieser Eigenschaft ist false. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields/) { get; } | Ruft die Liste der Felder von ods ab. |
| [PreserveString](../../aspose.cells/cells/preservestring/) { get; set; } | Liest oder legt einen Wert fest, der angibt, ob alle Arbeitsblattwerte als Zeichenfolgen erhalten bleiben. Standard ist false. |
| [Ranges](../../aspose.cells/cells/ranges/) { get; } | Ruft die Sammlung von [`Range`](../range/) Objekten ab, die zur Laufzeit erstellt werden. |
| [Rows](../../aspose.cells/cells/rows/) { get; } | Ruft die Sammlung von [`Row`](../row/) Objekten ab, die die einzelnen Zeilen in diesem Arbeitsblatt darstellen. |
| [StandardHeight](../../aspose.cells/cells/standardheight/) { get; set; } | Liest oder legt die Standardzeilenhöhe in diesem Arbeitsblatt in Punkten fest. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch/) { get; set; } | Liest oder legt die Standardzeilenhöhe in diesem Arbeitsblatt in Zoll fest. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels/) { get; set; } | Liest oder setzt die Standardzeilenhöhe in diesem Arbeitsblatt, in Pixel. |
| [StandardWidth](../../aspose.cells/cells/standardwidth/) { get; set; } | Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Zeichen. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch/) { get; set; } | Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Zoll. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels/) { get; set; } | Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Pixel. |
| [Style](../../aspose.cells/cells/style/) { get; set; } | Liest und setzt den Standardstil des Arbeitsblatts. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange/)(Range) | Fügt einen Bereichsobjektverweis zu Zellen hinzu |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle/)(int, Style, StyleFlag) | Wendet Formate für eine ganze Spalte an. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle/)(int, Style, StyleFlag) | Wendet Formate für eine ganze Zeile an. |
| [ApplyStyle](../../aspose.cells/cells/applystyle/)(Style, StyleFlag) | Wendet Formate für ein ganzes Arbeitsblatt an. |
| [CheckCell](../../aspose.cells/cells/checkcell/)(int, int) | Liest das [`Cell`](../cell/)‑Element oder null am angegebenen Zeilen‑ und Spaltenindex. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn/)(int) | Liest das [`Column`](../column/)‑Element oder null am angegebenen Spaltenindex. |
| [CheckRow](../../aspose.cells/cells/checkrow/)(int) | Liest das [`Row`](../row/)‑Element oder null am angegebenen Zeilenindex. |
| [Clear](../../aspose.cells/cells/clear/)() | Löscht alle Daten des Arbeitsblatts. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents)(CellArea) | Löscht den Inhalt eines Bereichs. |
| [ClearContents](../../aspose.cells/cells/clearcontents/#clearcontents_1)(int, int, int, int) | Löscht den Inhalt eines Bereichs. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats)(CellArea) | Löscht die Formatierung eines Bereichs. |
| [ClearFormats](../../aspose.cells/cells/clearformats/#clearformats_1)(int, int, int, int) | Löscht die Formatierung eines Bereichs. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells/)() | Löscht alle zusammengeführten Bereiche. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange)(CellArea) | Löscht Inhalt und Formatierung eines Bereichs. |
| [ClearRange](../../aspose.cells/cells/clearrange/#clearrange_1)(int, int, int, int) | Löscht Inhalt und Formatierung eines Bereichs. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue/)() | Konvertiert alle Zeichenkettendaten im Arbeitsblatt, wenn möglich, in numerische Werte. |
| [CopyColumn](../../aspose.cells/cells/copycolumn/)(Cells, int, int) | Kopiert Daten und Formate einer ganzen Spalte. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns)(Cells, int, int, int) | Kopiert Daten und Formate mehrerer Spalten. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_2)(Cells, int, int, int, int) | Kopiert Daten und Formate aller Spalten. |
| [CopyColumns](../../aspose.cells/cells/copycolumns/#copycolumns_1)(Cells, int, int, int, PasteOptions) | Kopiert Daten und Formate einer ganzen Spalte. |
| [CopyRow](../../aspose.cells/cells/copyrow/)(Cells, int, int) | Kopiert Daten und Formate einer ganzen Zeile. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows)(Cells, int, int, int) | Kopiert Daten und Formate einiger ganzer Zeilen. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_1)(Cells, int, int, int, CopyOptions) | Kopiert Daten und Formate einiger ganzer Zeilen. |
| [CopyRows](../../aspose.cells/cells/copyrows/#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | Kopiert Daten und Formate einiger ganzer Zeilen. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_2)(string) | Erstellt ein [`Range`](../range/)‑Objekt aus einer Adresse des Bereichs. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_3)(string, string) | Erstellt ein [`Range`](../range/)‑Objekt aus einem Zellbereich. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange)(int, int, bool) | Erstellt ein [`Range`](../range/)‑Objekt aus Zeilen von Zellen oder Spalten von Zellen. |
| [CreateRange](../../aspose.cells/cells/createrange/#createrange_1)(int, int, int, int) | Erstellt ein [`Range`](../range/)‑Objekt aus einem Zellbereich. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns)() | Löscht alle leeren Spalten, die keine Daten enthalten. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns/#deleteblankcolumns_1)(DeleteOptions) | Löscht alle leeren Spalten, die keine Daten enthalten. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows)() | Lösche alle leeren Zeilen, die keine Daten oder andere Objekte enthalten. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows/#deleteblankrows_1)(DeleteOptions) | Lösche alle leeren Zeilen, die keine Daten oder einige spezielle Objekte wie sichtbare Kommentare und Pivot-Tabellen enthalten. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn)(int) | Löscht eine Spalte. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn/#deletecolumn_1)(int, bool) | Löscht eine Spalte. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns_1)(int, int, bool) | Löscht mehrere Spalten. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns/#deletecolumns)(int, int, DeleteOptions) | Löscht mehrere Spalten. |
| [DeleteRange](../../aspose.cells/cells/deleterange/)(int, int, int, int, ShiftType) | Löscht einen Zellbereich und verschiebt Zellen gemäß der Verschiebungsoption. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow)(int) | Löscht eine Zeile. |
| [DeleteRow](../../aspose.cells/cells/deleterow/#deleterow_1)(int, bool) | Löscht eine Zeile. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows)(int, int) | Löscht mehrere Zeilen. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_2)(int, int, bool) | Löscht mehrere Zeilen im Arbeitsblatt. |
| [DeleteRows](../../aspose.cells/cells/deleterows/#deleterows_1)(int, int, DeleteOptions) | Löscht mehrere Zeilen im Arbeitsblatt. |
| [Dispose](../../aspose.cells/cells/dispose/)() | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn)(int) | Ermittelt die letzte Zelle in dieser Spalte. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn/#endcellincolumn_1)(int, int, int, int) | Ermittelt die letzte Zelle mit dem maximalen Spaltenindex in diesem Bereich. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow)(int) | Ermittelt die letzte Zelle in dieser Zeile. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow/#endcellinrow_1)(int, int, int, int) | Ermittelt die letzte Zelle mit dem maximalen Zeilenindex in diesem Bereich. |
| [ExportArray](../../aspose.cells/cells/exportarray/)(int, int, int, int) | Exportiert Daten aus der `Cells`-Auflistung in ein zweidimensionales Array-Objekt. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable)(int, int, int, int) | Exportiert Daten aus der `Cells`-Auflistung in ein DataTable-Objekt. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_2)(int, int, int, int, bool) | Exportiert Daten aus der `Cells`-Auflistung in ein DataTable-Objekt. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable/#exportdatatable_1)(int, int, int, int, ExportTableOptions) | Exportiert Daten aus der `Cells`-Auflistung in ein DataTable-Objekt. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring)(int, int, int, int) | Exportiert Daten aus der `Cells`-Auflistung in ein DataTable-Objekt. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring/#exportdatatableasstring_1)(int, int, int, int, bool) | Exportiert Daten aus der `Cells`-Auflistung in ein DataTable-Objekt. |
| [ExportList&lt;T&gt;](../../aspose.cells/cells/exportlist/)(int, int, int, int, ExportTableOptions) |  |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray/)(int, int, int, int) | Exportiert den Zellenwerttyp aus der `Cells`-Auflistung in ein zweidimensionales Array-Objekt. |
| [Find](../../aspose.cells/cells/find/#find)(object, Cell) | Findet die Zelle, die das Eingabeobjekt enthält. |
| [Find](../../aspose.cells/cells/find/#find_1)(object, Cell, FindOptions) | Findet die Zelle, die das Eingabeobjekt enthält. |
| [GetCell](../../aspose.cells/cells/getcell/)(int, int) | (**Obsolete.**) Gibt das [`Cell`](../cell/) Element oder null beim angegebenen Zeilen- und Spaltenindex zurück. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle)(int, int) | Ermittelt den Anzeigestil der angegebenen Zelle. |
| [GetCellDisplayStyle](../../aspose.cells/cells/getcelldisplaystyle/#getcelldisplaystyle_1)(int, int, BorderType) | Ermittelt den Anzeigestil der angegebenen Zelle. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle/)(int, int) | Ermittelt den Stil der angegebenen Zelle. |
| [GetCellsWithPlaceInCellPicture](../../aspose.cells/cells/getcellswithplaceincellpicture/)() | Ermittelt alle Zellen, die ein eingebettetes Bild enthalten. |
| [GetColumnOriginalWidthPoint](../../aspose.cells/cells/getcolumnoriginalwidthpoint/)(int) | (**Obsolete.**) Ermittelt die ursprüngliche Spaltenhöhe in Punkt, falls die Spalte ausgeblendet ist. |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth)(int) | Ermittelt die Breite (in Zeichen) der angegebenen Spalte in der Normalansicht. |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth/#getcolumnwidth_1)(int, bool, CellsUnitType) | Ermittelt die Spaltenbreite. |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch/)(int) | (**Obsolete.**) Ermittelt die Breite der angegebenen Spalte in der Normalansicht, in Zoll. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel)(int) | Ermittelt die Breite der angegebenen Spalte in der Normalansicht, in Pixel. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel/#getcolumnwidthpixel_1)(int, bool) | (**Obsolete.**) Gibt die Breite der angegebenen Spalte in der Normalansicht in Pixel zurück. |
| [GetDependents](../../aspose.cells/cells/getdependents/)(bool, int, int) | Alle Zellen erhalten, die sich auf die angegebene Zelle beziehen. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation/)(int, int, bool) | Gibt alle Zellen zurück, deren berechnetes Ergebnis von einer bestimmten Zelle abhängt. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator/)() | Gibt den Zellen‑Enumerator zurück. |
| [GetFirstDataRow](../../aspose.cells/cells/getfirstdatarow/)(int) | Gibt den Index der ersten Zeile der Zelle zurück, die Daten in der angegebenen Spalte enthält. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel/)(int) | Gibt die Gliederungsebene (nullbasiert) der Spalte zurück. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel/)(int) | Gibt die Gliederungsebene (nullbasiert) der Zeile zurück. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow/)(int) | Gibt den Index der letzten Zeile der Zelle zurück, die Daten in der angegebenen Spalte enthält. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/)() | Gibt die maximale gruppierte Spalten‑Gliederungsebene (nullbasiert) zurück. |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel/)() | Gibt die maximale gruppierte Zeilen‑Gliederungsebene (nullbasiert) zurück. |
| [GetMergedAreas](../../aspose.cells/cells/getmergedareas/)() | Gibt alle zusammengeführten Zellen zurück. |
| [GetRow](../../aspose.cells/cells/getrow/)(int) | (**Obsolete.**) Gibt das [`Row`](../row/)‑Element am angegebenen Zeilenindex der Zelle zurück. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator/)() | (**Obsolete.**) Gibt den Zeilen‑Enumerator zurück. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight)(int) | Gibt die Höhe einer angegebenen Zeile in Punkten zurück. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight/#getrowheight_1)(int, bool, CellsUnitType) | Gibt die Zeilenhöhe zurück. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch/)(int) | Gibt die Höhe einer angegebenen Zeile in Zoll zurück. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel/)(int) | Gibt die Höhe einer angegebenen Zeile in Pixel zurück. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint/)(int) | (**Obsolete.**) Gibt die ursprüngliche Zeilenhöhe in Punkten zurück, wenn die Zeile ausgeblendet ist. |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel/)(int) | Erhalte die Breite in verschiedenen Ansichtstypen. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight/)(int) | Gibt die Höhe einer angegebenen Zeile zurück. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch/)(int) | Gibt die Höhe einer angegebenen Zeile in Zoll zurück. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns)(int, int) | Gruppiert Spalten. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns/#groupcolumns_1)(int, int, bool) | Gruppiert Spalten. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows)(int, int) | Gruppiert Zeilen. |
| [GroupRows](../../aspose.cells/cells/grouprows/#grouprows_1)(int, int, bool) | Gruppiert Zeilen. |
| [HideColumn](../../aspose.cells/cells/hidecolumn/)(int) | Blendet eine Spalte aus. |
| [HideColumns](../../aspose.cells/cells/hidecolumns/)(int, int) | Blendet mehrere Spalten aus. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail/)(bool, int) | Klappt die gruppierten Zeilen/Spalten zusammen. |
| [HideRow](../../aspose.cells/cells/hiderow/)(int) | Blendet eine Zeile aus. |
| [HideRows](../../aspose.cells/cells/hiderows/)(int, int) | Blendet mehrere Zeilen aus. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_1)(double[], int, int, bool) | Importiert ein Array von double in ein Arbeitsblatt. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_3)(int[], int, int, bool) | Importiert ein Array von integer in ein Arbeitsblatt. |
| [ImportArray](../../aspose.cells/cells/importarray/#importarray_5)(string[], int, int, bool) | Importiert ein Array von string in ein Arbeitsblatt. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist/)(ArrayList, int, int, bool) | Importiert eine ArrayList von Daten in ein Arbeitsblatt. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv)(Stream, TxtLoadOptions, int, int) | Importiert eine CSV-Datei in die Zellen. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_2)(string, TxtLoadOptions, int, int) | Importiert eine CSV-Datei in die Zellen. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_1)(Stream, string, bool, int, int) | Importiert eine CSV-Datei in die Zellen. |
| [ImportCSV](../../aspose.cells/cells/importcsv/#importcsv_3)(string, string, bool, int, int) | Importiert eine CSV-Datei in die Zellen. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects)(ICollection, int, int, ImportTableOptions) | Importiert benutzerdefinierte Objekte. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects/#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | Importiert benutzerdefinierte Objekte. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_3)(IDataReader, int, int) | Importiert Daten aus einem IDataReader-Objekt. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_1)(DataTable, int, int, ImportTableOptions) | Importiert Daten aus einer benutzerdefinierten Datentabelle. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_2)(DataView, int, int, ImportTableOptions) | Importiert Daten aus einer Datenansicht. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata)(ICellsDataTable, int, int, ImportTableOptions) | Importiert Daten aus einer benutzerdefinierten Datentabelle. |
| [ImportData](../../aspose.cells/cells/importdata/#importdata_4)(IDataReader, int, int, ImportTableOptions) | Importiert Daten aus einem IDataReader-Objekt. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid)(DataGrid, int, int, bool) | Importiert ein DataGrid in ein Arbeitsblatt. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_1)(DataGrid, int, int, int, int, bool) | Importiert ein DataGrid in ein Arbeitsblatt. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid/#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | Importiert ein DataGrid in ein Arbeitsblatt. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring/)(DataGrid, int, int, bool) | Importiert ein DataGrid in ein Arbeitsblatt. Diese Methode versucht nicht, Text in numerische Werte zu konvertieren. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow/)(DataRow, int, int) | Importiert ein DataRow in die Excel-Datei. |
| [ImportDataView](../../aspose.cells/cells/importdataview/)(DataView, int, int) | Importiert ein DataView in ein Arbeitsblatt. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray/)(string[], int, int, bool) | Importiert ein Array von Formeln in ein Arbeitsblatt. |
| [ImportGridView](../../aspose.cells/cells/importgridview/)(GridView, int, int, ImportTableOptions) | Importiert ein grid view in diese Zellen. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray)(object[], int, int, bool) | Importiert ein Array von Daten in ein Arbeitsblatt. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray/#importobjectarray_1)(object[], int, int, bool, int) | Importiert ein Array von Daten in ein Arbeitsblatt. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray/#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn)(int) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn/#insertcolumn_1)(int, bool) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns)(int, int) | Fügt mehrere Spalten in das Arbeitsblatt ein. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_2)(int, int, bool) | Fügt mehrere Spalten in das Arbeitsblatt ein. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns/#insertcolumns_1)(int, int, InsertOptions) | Fügt mehrere Spalten in das Arbeitsblatt ein. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells/)(Range, int, int, ShiftType) | Einfügen des ausgeschnittenen Bereichs. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange)(CellArea, ShiftType) | Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_1)(CellArea, int, ShiftType) | Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption. |
| [InsertRange](../../aspose.cells/cells/insertrange/#insertrange_2)(CellArea, int, ShiftType, bool) | Fügt einen Zellbereich ein und verschiebt Zellen gemäß der Verschiebungsoption. |
| [InsertRow](../../aspose.cells/cells/insertrow/)(int) | Fügt eine neue Zeile in das Arbeitsblatt ein. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows)(int, int) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_2)(int, int, bool) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [InsertRows](../../aspose.cells/cells/insertrows/#insertrows_1)(int, int, InsertOptions) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn/)(int) | Prüft, ob die angegebene Spalte leer ist (enthält keine Daten). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden/)(int) | Überprüft, ob eine Spalte am angegebenen Index ausgeblendet ist. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled/)(int, int, int, int) | Überprüfen, ob der Bereich gelöscht werden kann. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden/)(int) | Überprüft, ob eine Zeile am angegebenen Index ausgeblendet ist. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap/)(string, int, int, string) | Link zu einer XML-Map. |
| [Merge](../../aspose.cells/cells/merge/#merge)(int, int, int, int) | Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen. |
| [Merge](../../aspose.cells/cells/merge/#merge_1)(int, int, int, int, bool) | Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen. |
| [Merge](../../aspose.cells/cells/merge/#merge_2)(int, int, int, int, bool, bool) | Führt einen angegebenen Zellbereich zu einer einzelnen Zelle zusammen. |
| [MoveRange](../../aspose.cells/cells/moverange/)(CellArea, int, int) | Verschiebt den Bereich. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates)() | Entfernt doppelte Zeilen im Blatt. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_1)(int, int, int, int) | Entfernt doppelte Werte im Bereich. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates/#removeduplicates_2)(int, int, int, int, bool, int[]) | Entfernt doppelte Daten des Bereichs. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas/)() | Entfernt alle Formeln und ersetzt sie durch den Wert der Formel. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting/)(CellArea) | Ruft die Zwischensummen‑Einstellung des Bereichs ab. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth/)(int, double) | Setzt die Breite der angegebenen Spalte in der Normalansicht. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch/)(int, double) | Setzt die Spaltenbreite in Zoll in der Normalansicht. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel/)(int, int) | Setzt die Spaltenbreite in Pixeln in der Normalansicht. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight/)(int, double) | Setzt die Höhe der angegebenen Zeile. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch/)(int, double) | Setzt die Zeilenhöhe in Zoll. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel/)(int, int) | Setzt die Zeilenhöhe in Pixeln. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel/)(int, int) | Setzt die Breite der Spalte in einer anderen Ansicht. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail/)(bool, int) | Erweitert die gruppierten Zeilen/Spalten. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal)(CellArea, int, ConsolidationFunction, int[]) | Erstellt Zwischensummen für den Bereich. |
| [Subtotal](../../aspose.cells/cells/subtotal/#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Erstellt Zwischensummen für den Bereich. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns/)(int, int, int, TxtLoadOptions) | Teilt den Inhalt in der angegebenen Spalte in mehrere Spalten auf.. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns/)(int, int) | Löst die Gruppierung von Spalten auf. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows)(int, int) | Löst die Gruppierung von Zeilen auf. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows/#ungrouprows_1)(int, int, bool) | Löst die Gruppierung von Zeilen auf. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn/)(int, double) | Blendet eine Spalte ein |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns/)(int, int, double) | Blendet mehrere Spalten ein. |
| [UnhideRow](../../aspose.cells/cells/unhiderow/)(int, double) | Blendet eine Zeile ein. |
| [UnhideRows](../../aspose.cells/cells/unhiderows/)(int, int, double) | Blendet die ausgeblendeten Zeilen ein. |
| [UnMerge](../../aspose.cells/cells/unmerge/)(int, int, int, int) | Löst einen angegebenen Bereich zusammengeführter Zellen auf. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsDemo
    {
        public static void CellsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Standardzeilenhöhe festlegen
            cells.StandardHeight = 20;
            // Zeilenhöhe festlegen
            cells.SetRowHeight(2, 20.5);

            // Standardspaltenbreite festlegen
            cells.StandardWidth = 15;
            // Spaltenbreite festlegen
            cells.SetColumnWidth(3, 12.57);

            // Zellen zusammenführen
            cells.Merge(5, 4, 2, 2);

            // Werte in Zellen einfügen
            cells[0, 0].PutValue(true);
            cells[0, 1].PutValue(1);
            cells[0, 2].PutValue("abc");

            // Daten exportieren
            object[,] arr = cells.ExportArray(0, 0, 10, 10);

            // Einige Eigenschaften demonstrieren
            Console.WriteLine("Total Cells Count: " + cells.Count);
            Console.WriteLine("Total Cells Count (Large): " + cells.CountLarge);
            Console.WriteLine("Min Row with Data: " + cells.MinDataRow);
            Console.WriteLine("Max Row with Data: " + cells.MaxDataRow);
            Console.WriteLine("Min Column with Data: " + cells.MinDataColumn);
            Console.WriteLine("Max Column with Data: " + cells.MaxDataColumn);

            // Durch Zellen iterieren
            IEnumerator enumerator = cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("CellsExample.xlsx");
            workbook.Save("CellsExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


