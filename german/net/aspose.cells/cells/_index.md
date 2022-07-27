---
title: Cells
second_title: Aspose.Cells für .NET-API-Referenz
description: Kapselt eine Sammlung von zellrelevanten Objekten wie zCell./cell Row./row ...etc.
type: docs
weight: 300
url: /de/net/aspose.cells/cells/
---
## Cells class

Kapselt eine Sammlung von zellrelevanten Objekten, wie z[`Cell`](../cell) ,[`Row`](../row) ...etc.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns) { get; } | Ruft die Sammlung von ab[`Column`](../column) Objekte, die die einzelnen Spalten in diesem Arbeitsblatt darstellen. |
| [Count](../../aspose.cells/cells/count) { get; } | Ruft die Gesamtzahl der instanziierten Cell-Objekte ab. |
| [CountLarge](../../aspose.cells/cells/countlarge) { get; } | Ruft die Gesamtzahl der instanziierten Cell-Objekte ab. |
| [FirstCell](../../aspose.cells/cells/firstcell) { get; } | Ruft die erste Zelle in diesem Arbeitsblatt ab. |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched) { get; set; } | Gibt an, dass Zeilenhöhe und Standardschrifthöhe mit übereinstimmen |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden) { get; set; } | Gibt an, ob die Zeile standardmäßig ausgeblendet ist. |
| [Item](../../aspose.cells/cells/item) { get; } | Ruft die ab[`Cell`](../cell) Element am angegebenen Zellenzeilenindex und Spaltenindex. (2 indexers) |
| [LastCell](../../aspose.cells/cells/lastcell) { get; } | Ruft die letzte Zelle in diesem Arbeitsblatt ab. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn) { get; } | Minimaler Spaltenindex der Zellen, die in der Sammlung instanziiert wurden (enthält nicht die Spalte , in der der Stil für die gesamte Spalte definiert ist, in der jedoch keine Zelle instanziiert wurde). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn) { get; } | Maximaler Spaltenindex der Zelle, die Daten enthält. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow) { get; } | Maximaler Zeilenindex der Zelle, die Daten enthält. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange) { get; } | Ruft den maximalen Bereich ab, der Daten, verbundene Zellen und Formen enthält. |
| [MaxRow](../../aspose.cells/cells/maxrow) { get; } | Maximaler Zeilenindex der Zelle, die Daten oder Stil enthält. |
| [MemorySetting](../../aspose.cells/cells/memorysetting) { get; set; } | Ruft die Speichernutzungsoption für diese Zellen ab oder legt sie fest. |
| [MergedCells](../../aspose.cells/cells/mergedcells) { get; } | Ruft die Sammlung verbundener Zellen ab. |
| [MinColumn](../../aspose.cells/cells/mincolumn) { get; } | Minimaler Spaltenindex der Zellen, die in der Sammlung instanziiert wurden (enthält nicht die Spalte , in der der Stil für die gesamte Spalte definiert ist, in der jedoch keine Zelle instanziiert wurde). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn) { get; } | Minimaler Spaltenindex der Zelle, die Daten enthält. |
| [MinDataRow](../../aspose.cells/cells/mindatarow) { get; } | Minimaler Zeilenindex der Zelle, die Daten enthält. |
| [MinRow](../../aspose.cells/cells/minrow) { get; } | Minimaler Zeilenindex der Zelle, die Daten oder Stil enthält. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading) { get; set; } | Ruft ab oder legt fest, ob das Zellendatenmodell Multi-Thread-Lesen unterstützen soll. Der Standardwert dieser Eigenschaft ist „false“. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields) { get; } | Ruft die Liste der Felder von ods ab. |
| [PreserveString](../../aspose.cells/cells/preservestring) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob alle Arbeitsblattwerte als Zeichenfolgen beibehalten werden. Standard ist falsch. |
| [Ranges](../../aspose.cells/cells/ranges) { get; } | Ruft die Sammlung von ab[`Range`](../range)zur Laufzeit erstellte Objekte. |
| [Rows](../../aspose.cells/cells/rows) { get; } | Ruft die Sammlung von ab[`Row`](../row) Objekte, die die einzelnen Zeilen in diesem Arbeitsblatt darstellen. |
| [StandardHeight](../../aspose.cells/cells/standardheight) { get; set; } | Ruft die Standardzeilenhöhe in diesem Arbeitsblatt in Punkteinheiten ab oder legt sie fest. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch) { get; set; } | Ruft die Standardzeilenhöhe in diesem Arbeitsblatt in Zoll ab oder legt sie fest. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels) { get; set; } | Ruft die Standardzeilenhöhe in diesem Arbeitsblatt in Pixeln ab oder legt sie fest. |
| [StandardWidth](../../aspose.cells/cells/standardwidth) { get; set; } | Ruft die Standardspaltenbreite im Arbeitsblatt in Zeicheneinheiten ab oder legt sie fest. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch) { get; set; } | Ruft die Standardspaltenbreite im Arbeitsblatt in Zoll ab oder legt sie fest. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels) { get; set; } | Ruft die Standardspaltenbreite im Arbeitsblatt in Pixeln ab oder legt sie fest. |
| [Style](../../aspose.cells/cells/style) { get; set; } | Ruft den Standardstil ab und legt ihn fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange)(Range) | Fügt eine Bereichsobjektreferenz zu cells hinzu |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle)(int, Style, StyleFlag) | Wendet Formate für eine ganze Spalte an. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle)(int, Style, StyleFlag) | Wendet Formate für eine ganze Zeile an. |
| [ApplyStyle](../../aspose.cells/cells/applystyle)(Style, StyleFlag) | Wendet Formate auf ein ganzes Arbeitsblatt an. |
| [CheckCell](../../aspose.cells/cells/checkcell)(int, int) | Ruft die ab[`Cell`](../cell) element oder null am angegebenen Zellenzeilenindex und Spaltenindex. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn)(int) | Ruft die ab[`Column`](../column) element oder null am angegebenen Spaltenindex. |
| [CheckRow](../../aspose.cells/cells/checkrow)(int) | Ruft die ab[`Row`](../row) Element oder am angegebenen Zellenzeilenindex. |
| [Clear](../../aspose.cells/cells/clear)() | Löscht alle Zellen- und Zeilenobjekte. |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents)(CellArea) | Löscht den Inhalt eines Bereichs. |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents_1)(int, int, int, int) | Löscht den Inhalt eines Bereichs. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats)(CellArea) | Löscht die Formatierung eines Bereichs. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats_1)(int, int, int, int) | Löscht die Formatierung eines Bereichs. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells)() | Löscht alle zusammengeführten Bereiche. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange)(CellArea) | Löscht Inhalt und Formatierung eines Bereichs. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange_1)(int, int, int, int) | Löscht Inhalt und Formatierung eines Bereichs. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue)() | Konvertiert Zeichenfolgendaten in Zellen nach Möglichkeit in numerische Werte. |
| [CopyColumn](../../aspose.cells/cells/copycolumn)(Cells, int, int) | Kopiert Daten und Formate einer ganzen Spalte. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns)(Cells, int, int, int) | Kopiert Daten und Formate einer ganzen Spalte. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_2)(Cells, int, int, int, int) | Kopiert Daten und Formate der ganzen Spalten. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_1)(Cells, int, int, int, PasteOptions) | Kopiert Daten und Formate einer ganzen Spalte. |
| [CopyRow](../../aspose.cells/cells/copyrow)(Cells, int, int) | Kopiert Daten und Formate einer ganzen Zeile. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows)(Cells, int, int, int) | Kopiert Daten und Formate einiger ganzer Zeilen. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_1)(Cells, int, int, int, CopyOptions) | Kopiert Daten und Formate einiger ganzer Zeilen. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | Kopiert Daten und Formate einiger ganzer Zeilen. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_2)(string) | Erstellt ein[`Range`](../range) Objekt aus einer Adresse des Bereichs. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_3)(string, string) | Erstellt ein[`Range`](../range) Objekt aus einer Reihe von Zellen. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange)(int, int, bool) | Erstellt ein[`Range`](../range) Objekt aus Zeilen von Zellen oder Spalten von Zellen. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_1)(int, int, int, int) | Erstellt ein[`Range`](../range) Objekt aus einer Reihe von Zellen. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns)() | Löschen Sie alle leeren Spalten, die keine Daten enthalten. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns_1)(DeleteOptions) | Löschen Sie alle leeren Spalten, die keine Daten enthalten. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows)() | Löschen Sie alle leeren Zeilen, die keine Daten enthalten. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows_1)(DeleteOptions) | Löschen Sie alle leeren Zeilen, die keine Daten enthalten. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn)(int) | Löscht eine Spalte. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn_1)(int, bool) | Löscht eine Spalte. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns)(int, int, bool) | Löscht mehrere Spalten. |
| [DeleteRange](../../aspose.cells/cells/deleterange)(int, int, int, int, ShiftType) | Löscht einen Bereich von Zellen und verschiebt Zellen entsprechend der Verschiebeoption. |
| [DeleteRow](../../aspose.cells/cells/deleterow)(int) | Löscht eine Zeile. |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows)(int, int) | Löscht mehrere Zeilen. |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows_1)(int, int, bool) | Löscht mehrere Zeilen im Arbeitsblatt. |
| [Dispose](../../aspose.cells/cells/dispose)() | Führt anwendungsdefinierte Aufgaben aus, die mit dem Freigeben, Freigeben oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn)(short) | Ruft die letzte Zelle in dieser Spalte ab. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn_1)(int, int, short, short) | Ruft die letzte Zelle mit maximalem Spaltenindex in diesem Bereich ab. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow)(int) | Ruft die letzte Zelle in dieser Zeile ab. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow_1)(int, int, int, int) | Ruft die letzte Zelle mit maximalem Zeilenindex in diesem Bereich ab. |
| [ExportArray](../../aspose.cells/cells/exportarray)(int, int, int, int) | Exportiert Daten in die[`Cells`](../cells) Sammlung in ein zweidimensionales Array-Objekt. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable)(int, int, int, int) | Exportiert Daten in die[`Cells`](../cells) Sammlung zu aDataTable Objekt. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_2)(int, int, int, int, bool) | Exportiert Daten in die[`Cells`](../cells) Sammlung zu aDataTable Objekt. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_1)(int, int, int, int, ExportTableOptions) | Exportiert Daten in die[`Cells`](../cells) Sammlung zu aDataTable Objekt. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring)(int, int, int, int) | Exportiert Daten in die[`Cells`](../cells) Sammlung zu aDataTable Objekt. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring_1)(int, int, int, int, bool) | Exportiert Daten in die[`Cells`](../cells) Sammlung zu aDataTable Objekt. |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray)(int, int, int, int) | Exportiert den Zellenwerttyp in die[`Cells`](../cells) Sammlung in ein zweidimensionales Array-Objekt. |
| [Find](../../aspose.cells/cells/find#find)(object, Cell) | Findet die Zelle, die das Eingabeobjekt enthält. |
| [Find](../../aspose.cells/cells/find#find_1)(object, Cell, FindOptions) | Findet die Zelle, die das Eingabeobjekt enthält. |
| [GetCell](../../aspose.cells/cells/getcell)(int, int) | Ruft die ab[`Cell`](../cell) element oder null am angegebenen Zellenzeilenindex und Spaltenindex. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle)(int, int) | Ruft den Stil der angegebenen Zelle ab. |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth)(int) | Ruft die Breite der angegebenen Spalte in der normalen Ansicht ab |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch)(int) | Ruft die Breite der angegebenen Spalte in der Normalansicht in Zolleinheiten ab. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel)(int) | Ruft die Breite der angegebenen Spalte in der Normalansicht in Pixeleinheiten ab. |
| [GetDependents](../../aspose.cells/cells/getdependents)(bool, int, int) | Alle Zellen abrufen, die sich auf die bestimmte Zelle beziehen. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation)(int, int, bool) | Ruft alle Zellen ab, deren berechnetes Ergebnis von einer bestimmten Zelle abhängt. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator)() | Ruft den Zellenzähler ab. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel)(int) | Ruft die Gliederungsebene (nullbasiert) der Spalte ab. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel)(int) | Ruft die Gliederungsebene (nullbasiert) der Zeile ab. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow)(int) | Ruft den letzten Zeilenindex der Zelle ab, die Daten in der angegebenen Spalte enthält. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel)() | Ruft die maximale gruppierte Spaltengliederungsebene ab (nullbasiert). |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel)() | Ruft die maximale gruppierte Zeilenumrissebene ab (nullbasiert). |
| [GetRow](../../aspose.cells/cells/getrow)(int) | Ruft die ab[`Row`](../row) Element am angegebenen Zellenzeilenindex. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator)() | Ruft den Zeilen-Enumerator ab. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight)(int) | Ruft die Höhe einer angegebenen Zeile ab. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch)(int) | Ruft die Höhe einer angegebenen Zeile in der Einheit Zoll ab. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel)(int) | Ruft die Höhe einer angegebenen Zeile in Pixeleinheiten ab. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint)(int) | Ruft die Höhe der ursprünglichen Zeile in Punkteinheit ab, wenn die Zeile ausgeblendet ist |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel)(int) | Holen Sie sich die Breite in einem anderen Ansichtstyp. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight)(int) | Ruft die Höhe einer angegebenen Zeile ab. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch)(int) | Ruft die Höhe einer angegebenen Zeile in der Einheit Zoll ab. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns)(int, int) | Gruppiert Spalten. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns_1)(int, int, bool) | Gruppiert Spalten. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows)(int, int) | Gruppiert Zeilen. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows_1)(int, int, bool) | Gruppiert Zeilen. |
| [HideColumn](../../aspose.cells/cells/hidecolumn)(int) | Blendet eine Spalte aus. |
| [HideColumns](../../aspose.cells/cells/hidecolumns)(int, int) | Mehrere Spalten ausblenden. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail)(bool, int) | Reduziert die gruppierten Zeilen/Spalten. |
| [HideRow](../../aspose.cells/cells/hiderow)(int) | Blendet eine Zeile aus. |
| [HideRows](../../aspose.cells/cells/hiderows)(int, int) | Blendet mehrere Zeilen aus. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_1)(double[], int, int, bool) | Importiert ein Array von Double in ein Arbeitsblatt. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_3)(int[], int, int, bool) | Importiert ein Integer-Array in ein Arbeitsblatt. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_5)(string[], int, int, bool) | Importiert ein String-Array in ein Arbeitsblatt. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist)(ArrayList, int, int, bool) | Importiert eine Arrayliste von Daten in ein Arbeitsblatt. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv)(Stream, TxtLoadOptions, int, int) | Importieren Sie eine CSV-Datei in die Zellen. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_2)(string, TxtLoadOptions, int, int) | Importieren Sie eine CSV-Datei in die Zellen. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_1)(Stream, string, bool, int, int) | Importieren Sie eine CSV-Datei in die Zellen. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_3)(string, string, bool, int, int) | Importieren Sie eine CSV-Datei in die Zellen. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects)(ICollection, int, int, ImportTableOptions) | Importiert benutzerdefinierte Objekte. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | Importiert benutzerdefinierte Objekte. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_3)(IDataReader, int, int) | Importiert Daten von aIDataReader Objekt. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_1)(DataTable, int, int, ImportTableOptions) | Daten aus benutzerdefinierter Datentabelle importieren. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_2)(DataView, int, int, ImportTableOptions) | Daten aus Datenansicht importieren. |
| [ImportData](../../aspose.cells/cells/importdata#importdata)(ICellsDataTable, int, int, ImportTableOptions) | Daten aus benutzerdefinierter Datentabelle importieren. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_4)(IDataReader, int, int, ImportTableOptions) | Importiert Daten von aIDataReader Objekt. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid)(DataGrid, int, int, bool) | Importiert aDataGrid in ein Arbeitsblatt. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_1)(DataGrid, int, int, int, int, bool) | Importiert aDataGrid in ein Arbeitsblatt. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | Importiert aDataGrid in ein Arbeitsblatt. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring)(DataGrid, int, int, bool) | Importiert aDataGrid in ein Arbeitsblatt. Diese Methode versucht nicht, Text in numerische Werte umzuwandeln. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow)(DataRow, int, int) | Importiert eine DataRow in die Excel-Datei. |
| [ImportDataView](../../aspose.cells/cells/importdataview#importdataview_3)(DataView, int, int) | Importiert aDataView in ein Arbeitsblatt. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray)(string[], int, int, bool) | Importiert ein Array von Formeln in ein Arbeitsblatt. |
| [ImportGridView](../../aspose.cells/cells/importgridview)(GridView, int, int, ImportTableOptions) | Importiert eine Rasteransicht in diese Zellen. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray)(object[], int, int, bool) | Importiert ein Array von Daten in ein Arbeitsblatt. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray_1)(object[], int, int, bool, int) | Importiert ein Array von Daten in ein Arbeitsblatt. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn)(int) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn_1)(int, bool) | Fügt eine neue Spalte in das Arbeitsblatt ein. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns)(int, int) | Fügt einige Spalten in das Arbeitsblatt ein. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns_1)(int, int, bool) | Fügt einige Spalten in das Arbeitsblatt ein. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells)(Range, int, int, ShiftType) | Schnittbereich einfügen. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange)(CellArea, ShiftType) | Fügt einen Bereich von Zellen ein und verschiebt Zellen entsprechend der Verschiebeoption. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_1)(CellArea, int, ShiftType) | Fügt einen Bereich von Zellen ein und verschiebt Zellen entsprechend der Verschiebeoption. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_2)(CellArea, int, ShiftType, bool) | Fügt einen Bereich von Zellen ein und verschiebt Zellen entsprechend der Verschiebeoption. |
| [InsertRow](../../aspose.cells/cells/insertrow)(int) | Fügt eine neue Zeile in das Arbeitsblatt ein. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows)(int, int) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_2)(int, int, bool) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_1)(int, int, InsertOptions) | Fügt mehrere Zeilen in das Arbeitsblatt ein. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn)(int) | Prüft, ob die angegebene Spalte leer ist (enthält keine Daten). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden)(int) | Überprüft, ob eine Spalte am angegebenen Index ausgeblendet ist. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled)(int, int, int, int) | Prüfen, ob der Bereich gelöscht werden konnte. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden)(int) | Überprüft, ob eine Zeile am angegebenen Index ausgeblendet ist. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap)(string, int, int, string) | Link zu einer XML-Karte. |
| [Merge](../../aspose.cells/cells/merge#merge)(int, int, int, int) | Führt einen angegebenen Zellbereich zu einer einzigen Zelle zusammen. |
| [Merge](../../aspose.cells/cells/merge#merge_1)(int, int, int, int, bool) | Führt einen angegebenen Zellbereich zu einer einzigen Zelle zusammen. |
| [Merge](../../aspose.cells/cells/merge#merge_2)(int, int, int, int, bool, bool) | Führt einen angegebenen Zellbereich zu einer einzigen Zelle zusammen. |
| [MoveRange](../../aspose.cells/cells/moverange)(CellArea, int, int) | Verschiebt den Bereich. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates)() | Entfernt doppelte Zeilen im Blatt. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_1)(int, int, int, int) | Entfernt doppelte Werte im Bereich. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_2)(int, int, int, int, bool, int[]) | Entfernt doppelte Daten des Bereichs. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas)() | Entfernt alle Formeln und ersetzt sie durch den Wert der Formel. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting)(CellArea) | Ruft die Zwischensummeneinstellung des Bereichs ab. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth)(int, double) | Legt die Breite der angegebenen Spalte in der Normalansicht fest. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch)(int, double) | Legt die Spaltenbreite in der Normalansicht in Zoll fest. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel)(int, int) | Legt die Spaltenbreite in der Einheit Pixel in der Normalansicht fest. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight)(int, double) | Legt die Höhe der angegebenen Zeile fest. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch)(int, double) | Legt die Zeilenhöhe in Zoll fest. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel)(int, int) | Legt die Zeilenhöhe in Pixeleinheiten fest. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel)(int, int) | Legt die Breite der Spalte in verschiedenen Ansichten fest. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail)(bool, int) | Erweitert die gruppierten Zeilen/Spalten. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal)(CellArea, int, ConsolidationFunction, int[]) | Erstellt Zwischensummen für den Bereich. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Erstellt Zwischensummen für den Bereich. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns)(int, int, int, TxtLoadOptions) | Teilt den Text in der Spalte in Spalten auf. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns)(int, int) | Hebt die Gruppierung von Spalten auf. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows)(int, int) | Hebt die Gruppierung von Zeilen auf. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows_1)(int, int, bool) | Hebt die Gruppierung von Zeilen auf. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn)(int, double) | Blendet eine Spalte ein |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns)(int, int, double) | Mehrere Spalten einblenden. |
| [UnhideRow](../../aspose.cells/cells/unhiderow)(int, double) | Blendet eine Zeile ein. |
| [UnhideRows](../../aspose.cells/cells/unhiderows)(int, int, double) | Blendet die ausgeblendeten Zeilen ein. |
| [UnMerge](../../aspose.cells/cells/unmerge)(int, int, int, int) | Hebt die Zusammenführung eines bestimmten Bereichs verbundener Zellen auf. |

### Beispiele

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//Standard-Zeilenhöhe festlegen
cells.StandardHeight = 20;
//Zeilenhöhe festlegen
cells.SetRowHeight(2, 20.5);

//Standardspaltenbreite festlegen
cells.StandardWidth = 15;
//Spaltenbreite festlegen
cells.SetColumnWidth(3, 12.57);

//Zellen verbinden
cells.Merge(5, 4, 2, 2);

//Legen Sie Werte in Zellen
cells[0, 0].PutValue(true);
cells[0, 1].PutValue(1);
cells[0, 2].PutValue("abc");

//Daten exportieren
object[,] arr = cells.ExportArray(0, 0, 10, 10);

[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells

'Legen Sie die Standardzeilenhöhe fest
cells.StandardHeight = 20
'Zeilenhöhe einstellen
cells.SetRowHeight(2, 20.5)

'Legen Sie die Standardspaltenbreite fest
cells.StandardWidth = 15
'Spaltenbreite einstellen
cells.SetColumnWidth(3, 12.57)

'Zellen verbinden
cells.Merge(5, 4, 2, 2)

'Daten exportieren
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
