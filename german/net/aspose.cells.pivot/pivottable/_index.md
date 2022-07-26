---
title: PivotTable
second_title: Aspose.Cells für .NET-API-Referenz
description: Zusammenfassende Beschreibung für PivotTable.
type: docs
weight: 4690
url: /de/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

Zusammenfassende Beschreibung für PivotTable.

```csharp
public class PivotTable : IDisposable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription) { get; set; } | Ruft die Beschreibung des Alternativtexts ab |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle) { get; set; } | Ruft den Titel des Altertexts ab |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype) { get; set; } | Ruft den automatischen Formattyp der PivotTable ab. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields) { get; } | Gibt ein PivotFields-Objekt zurück, das alle Felder im PivotTable-Bericht enthält |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields) { get; } | Gibt ein PivotFields-Objekt zurück, das derzeit als Spaltenfelder angezeigt wird. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand) { get; set; } | Gibt an, ob der PivotTable-Bericht Gesamtsummen für Spalten anzeigt. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption) { get; set; } | Ruft die Spaltenüberschrift der PivotTable ab. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange) { get; } | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Spaltenbereich im PivotTable-Bericht enthält. Schreibgeschützt. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort) { get; set; } | Gibt an, ob beim Sortieren von Daten die integrierte benutzerdefinierte Liste berücksichtigt wird |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange) { get; } | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der die Daten area in der Liste zwischen der Kopfzeile und der Einfügezeile enthält. Schreibgeschützt. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield) { get; } | Ruft ein PivotField-Objekt ab, das alle Datenfelder in einer PivotTable darstellt. Schreibgeschützt. Es wäre nur init, wenn zwei oder mehr Datenfelder in den DataPiovtFiels vorhanden sind. Es wird nur verwendet, um DataPivotField zur Zeile/Spalte der PivotTable hinzuzufügen Bereich . Standard ist im Zeilenbereich. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields) { get; } | Ruft ein PivotField-Objekt ab, das alle Datenfelder in einer PivotTable darstellt. Schreibgeschützt. Es wäre nur init, wenn zwei oder mehr Datenfelder in den DataPiovtFiels vorhanden sind. Es wird nur verwendet, um DataPivotField zur Zeile/Spalte der PivotTable hinzuzufügen Bereich . Standard ist im Zeilenbereich. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource) { get; set; } | Ruft die Datenquelle der Pivot-Tabelle ab und legt sie fest. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring) { get; set; } | Gibt an, ob der PivotTable-Bericht eine benutzerdefinierte Zeichenfolge in Zellen anzeigt, die Fehler enthalten. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems) { get; set; } | Gibt an, ob Elemente in den Zeilen- und Spaltenbereichen sichtbar sind , wenn der Datenbereich der PivotTable leer ist. Der Standardwert ist true. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring) { get; set; } | Gibt an, ob der PivotTable-Bericht eine benutzerdefinierte Zeichenfolge in Zellen anzeigt, die Nullwerte enthalten. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting) { get; set; } | Gibt einen booleschen Wert an, der angibt, ob der Benutzer berechtigt ist, die Zellen im Datenbereich der Pivottable zu bearbeiten. Zellbearbeitung im Wertebereich aktivieren |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown) { get; set; } | Ruft ab, ob Drilldown aktiviert ist. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog) { get; set; } | Gibt an, ob das Dialogfeld PivotTable-Feld verfügbar ist , wenn der Benutzer auf das PivotTable-Feld doppelklickt. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist) { get; set; } | Ruft ab, ob die Feldliste für die PivotTable aktiviert ist. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard) { get; set; } | Gibt an, ob der PivotTable-Assistent verfügbar ist. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring) { get; set; } | Ruft die Zeichenfolge ab, die in Zellen angezeigt wird, die error enthalten, wenn die DisplayErrorString-Eigenschaft wahr ist. Der Standardwert ist eine leere Zeichenfolge. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource) { get; } | Ruft die externe Verbindungsdatenquelle ab. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending) { get; set; } | Gibt einen booleschen Wert an, der angibt, ob Felder in der PivotTable in der Feldliste in einer nicht standardmäßigen Reihenfolge sortiert sind. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname) { get; set; } | Gibt die Beschriftung der Textzeichenfolge zurück, die in der Spalten- oder Zeilenüberschrift der Gesamtsumme angezeigt wird. Der Standardwert ist die Zeichenfolge „Gesamtsumme“. |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows) { get; set; } | Gibt an, ob leere Zeilen hinzugefügt werden sollen. Diese Eigenschaft gilt nur für die PivotTable-Autoformattypen, bei denen leere Zeilen hinzugefügt werden müssen. |
| [Indent](../../aspose.cells.pivot/pivottable/indent) { get; set; } | Gibt das Einzugsinkrement für die kompakte Achse an und kann verwendet werden, um das Berichtslayout auf kompakte Form einzustellen. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat) { get; set; } | Gibt an, ob der PivotTable-Bericht automatisch formatiert wird. Kontrollkästchen „Tabelle automatisch formatieren“ in der Pivottable-Option für Excel 2003 Kontrollkästchen „Spaltenbreite bei Aktualisierung automatisch anpassen“ in den Pivot-Tabellenoptionen: Layoutformat für Excel 2007 |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible) { get; set; } | Gibt an, ob die PivotTable beim Aktualisieren der PivotTable mit Excel2003 kompatibel ist, wenn wahr, muss eine Zeichenfolge kleiner oder gleich 255 Zeichen sein, wenn die Zeichenfolge also länger als 255 Zeichen ist, wird sie abgeschnitten. Bei „false“ hat eine Zeichenfolge die oben genannte Einschränkung nicht. Der Standardwert ist „true“. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones) { get; set; } | Gibt an, ob der PivotTable-Bericht das klassische PivotTable-Layout anzeigt. (ermöglicht das Ziehen von Feldern im Raster) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters) { get; set; } | Gibt einen booleschen Wert an, der angibt, ob für die Felder einer PivotTable mehrere Filter festgelegt werden können. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected) { get; set; } | Gibt an, ob die PivotTable ausgewählt ist. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles) { get; set; } | Ein Bit, das angibt, ob Pivot-Elementbeschriftungen auf der Zeilenachse auf jeder gedruckten Seite für Pivot-Felder in Tabellenform wiederholt werden. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate) { get; set; } | Gibt an, ob der PivotTable-Bericht nur auf Anforderung des Benutzers neu berechnet wird. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels) { get; set; } | Gibt an, ob die äußeren Zeilenelemente, Spaltenelemente, Zwischensummen, und Gesamtsummenbeschriftungen des angegebenen PivotTable-Berichts verbundene Zellen verwenden. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit) { get; set; } | Gibt einen booleschen Wert an, der angibt, ob für die Felder einer PivotTable mehrere Filter festgelegt werden können. |
| [Name](../../aspose.cells.pivot/pivottable/name) { get; set; } | Ruft den Namen der PivotTable ab |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring) { get; set; } | Ruft die Zeichenfolge ab, die in Zellen angezeigt wird, die Nullwerte enthalten , wenn die DisplayNullString-Eigenschaft wahr ist. Der Standardwert ist eine leere Zeichenfolge. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder) { get; set; } | Ruft die Reihenfolge ab, in der Seitenfelder zum Layout des PivotTable-Berichts hinzugefügt werden. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields) { get; } | Gibt ein PivotFields-Objekt zurück, das derzeit als Seitenfelder angezeigt wird. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount) { get; set; } | Ruft die Anzahl der Seitenfelder in jeder Spalte oder Zeile im PivotTable-Bericht ab. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters) { get; } | Gibt ein PivotFilterCollection-Objekt zurück. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions) { get; } | Ruft die Formatbedingungen der Pivot-Tabelle ab. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename) { get; set; } | Ruft den schwenkbaren Stilnamen ab und legt ihn fest. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype) { get; set; } | Ruft den integrierten Pivot-Tabellenstil ab und legt ihn fest. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting) { get; set; } | Gibt an, ob die Formatierung beibehalten wird, wenn die PivotTable aktualisiert oder neu berechnet wird. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill) { get; set; } | Gibt einen booleschen Wert an, der angibt, ob Bohrindikatoren gedruckt werden sollen. Schaltflächen zum Erweitern/Reduzieren drucken, wenn sie auf einer Pivottable angezeigt werden. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles) { get; set; } | Gibt an, ob die Drucktitel für das Arbeitsblatt basierend auf dem PivotTable-Bericht festgelegt werden. Der Standardwert ist false. |
| [RefreshDataFlag](../../aspose.cells.pivot/pivottable/refreshdataflag) { get; set; } | Gibt an, ob Daten aktualisiert werden oder nicht. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile) { get; set; } | Gibt an, ob Daten beim Öffnen einer Datei aktualisiert werden. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate) { get; } | Ruft das Datum ab, an dem die PivotTable zuletzt aktualisiert wurde. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho) { get; } | Ruft den Namen des Benutzers ab, der die PivotTable zuletzt aktualisiert hat |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields) { get; } | Gibt ein PivotFields-Objekt zurück, das derzeit als Zeilenfelder angezeigt wird. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand) { get; set; } | Gibt an, ob der PivotTable-Bericht Gesamtsummen für Zeilen anzeigt. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption) { get; set; } | Ruft die Zeilenkopfzeile der PivotTable ab. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange) { get; } | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Zeilenbereich im PivotTable-Bericht enthält. Schreibgeschützt. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata) { get; set; } | Gibt an, ob Daten für den PivotTable-Bericht mit der Arbeitsmappe gespeichert werden. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips) { get; set; } | Gibt einen booleschen Wert an, der angibt, ob QuickInfos für PivotTable-Datenzellen angezeigt werden sollen. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill) { get; set; } | Ruft ab, ob Schaltflächen zum Erweitern/Reduzieren angezeigt werden. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol) { get; set; } | Gibt einen booleschen Wert an, der angibt, ob leere Spalten in die Tabelle aufgenommen werden sollen |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow) { get; set; } | Gibt einen booleschen Wert an, der angibt, ob leere Zeilen in die Tabelle aufgenommen werden sollen. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips) { get; set; } | Gibt einen booleschen Wert an, der angibt, ob Informationen zu Elementeigenschaften in PivotTable-QuickInfos weggelassen werden sollen. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader) { get; set; } | Gibt an, ob auf die Spaltenüberschrift in der Pivot-Tabelle der Stil angewendet werden soll. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes) { get; set; } | Gibt an, ob Spaltenstreifenformatierung angewendet wird. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn) { get; set; } | Gibt an, ob Spaltenstreifenformatierung angewendet wird. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader) { get; set; } | Gibt an, ob auf die Zeilenüberschrift in der Pivot-Tabelle der Stil angewendet werden soll. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes) { get; set; } | Gibt an, ob Zeilenstreifenformatierung angewendet wird. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption) { get; set; } | Gibt an, ob Zeilenüberschriften im PivotTable-Bericht angezeigt werden Gibt an, ob Feldbeschriftungen und Filter-Dropdowns angezeigt werden |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow) { get; set; } | Gibt einen booleschen Wert an, der angibt, ob die Wertezeile angezeigt wird. zeigt die Wertezeile |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems) { get; set; } | Gibt an, ob ausgeblendete Seitenfeldelemente im PivotTable-Bericht in Zeilen- und Spaltenzwischensummen, Blocksummen und Gesamtsummen enthalten sind. Der Standardwert ist False. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1) { get; } | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den gesamten PivotTable-Bericht enthält, aber keine Seitenfelder enthält. Schreibgeschützt. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2) { get; } | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den gesamten PivotTable-Bericht enthält, enthält Seitenfelder. Schreibgeschützt. |
| [Tag](../../aspose.cells.pivot/pivottable/tag) { get; set; } | Ruft eine mit dem PivotTable-Bericht gespeicherte Zeichenfolge ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield)(string, string) | Fügt ein berechnetes Feld zum Pivot-Feld hinzu und zieht es in den Datenbereich. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield_1)(string, string, bool) | Fügt dem Pivot-Feld ein berechnetes Feld hinzu. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_1)(PivotFieldType, int) | Fügt das Feld dem spezifischen Bereich hinzu. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea)(PivotFieldType, PivotField) | Fügt das Feld dem spezifischen Bereich hinzu. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_2)(PivotFieldType, string) | Fügt das Feld dem spezifischen Bereich hinzu. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata)() | Berechnet Pivottable-Daten in Zellen. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange)() | Berechnet den Pivottable-Bereich. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource)(string[]) | Pivottable-Quelldaten festlegen. Sheet1!$A$1:$C$3 |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata)() | Daten und Formatierung von PivotTable löschen |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle)(PivotTable) | Kopiert den benannten Stil aus einer anderen Pivot-Tabelle. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose)() | Führt anwendungsdefinierte Aufgaben aus, die mit dem Freigeben, Freigeben oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [Fields](../../aspose.cells.pivot/pivottable/fields)(PivotFieldType) | Ruft die spezifischen Felder nach Feldtyp ab. |
| [Format](../../aspose.cells.pivot/pivottable/format)(int, int, Style) | Formatieren Sie die Zelle im schwenkbaren Bereich |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall)(Style) | Alle Zellen im schwenkbaren Bereich formatieren |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow)(int, Style) | Formatieren Sie die Zeilendaten im schwenkbaren Bereich |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname)(string) | Ruft das Cell-Objekt anhand des Anzeigenamens von PivotField ab. |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren)() | Ruft die untergeordneten Pivot-Tabellen ab, die diese PivotTable-Daten als Datenquelle verwenden. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks)() | Pivot-Tabellenzeilen-Indexliste der horizontalen Seitenumbrüche abrufen |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource)() | Pivottable-Quelldaten abrufen. |
| [Move](../../aspose.cells.pivot/pivottable/move#move_1)(string) | Verschiebt die PivotTable an eine andere Position im Arbeitsblatt. |
| [Move](../../aspose.cells.pivot/pivottable/move#move)(int, int) | Verschiebt die PivotTable an eine andere Position im Arbeitsblatt. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata)() | Aktualisiert die Daten und Einstellungen der Pivottable aus ihrer Datenquelle. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_1)(PivotFieldType, int) | Entfernt ein Feld aus einem bestimmten Feldbereich |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield)(PivotFieldType, PivotField) | Feld aus bestimmtem Feldbereich entfernen |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_2)(PivotFieldType, string) | Entfernt ein Feld aus einem bestimmten Feldbereich |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield_1)(int) | Legt die automatische Feldgruppe nach PivotTable fest. |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield)(PivotField) | Legt die automatische Feldgruppe nach PivotTable fest. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_3)(int, DateTime, DateTime, ArrayList, int) | Legt die manuelle Feldgruppe durch die PivotTable fest. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_2)(int, double, double, ArrayList, double) | Legt die manuelle Feldgruppe durch die PivotTable fest. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_1)(PivotField, DateTime, DateTime, ArrayList, int) | Legt die manuelle Feldgruppe durch die PivotTable fest. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield)(PivotField, double, double, ArrayList, double) | Legt die manuelle Feldgruppe durch die PivotTable fest. |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup_1)(int) | Setzt die Gruppierung durch die PivotTable aufheben |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup)(PivotField) | Setzt die Gruppierung durch die PivotTable aufheben |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform)() | Layouts der PivotTable in kompakter Form. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform)() | Layouts der PivotTable in Gliederungsform. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform)() | Layouts der PivotTable in tabellarischer Form. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage)(PivotField) | Alle Berichtsfilterseiten nach PivotField anzeigen, das PivotField muss sich in den PageFields befinden. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex)(int) | Alle Berichtsfilterseiten gemäß dem Positionsindex in den PageFields anzeigen |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname)(string) | Alle Berichtsfilterseiten gemäß dem Namen des PivotFields anzeigen, das PivotField muss sich in den PageFields befinden. |

### Beispiele

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Attribute von PivotField ändern
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

//PivotFilter hinzufügen
int index = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[index];
filter.AutoFilter.FilterTop10(0, false, false, 2);

//PivotFormatCondition hinzufügen
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;

pivot.RefreshData();
pivot.CalculateData();

// Mach dein Geschäft

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'PivotFilter hinzufügen
Dim filterIndex As Int32 = pivot.PivotFilters.Add(0, PivotFilterType.Count)
Dim filter As PivotFilter = pivot.PivotFilters(filterIndex)
filter.AutoFilter.FilterTop10(0, False, False, 2)

'Fügen Sie PivotFormatCondition hinzu
Dim formatIndex As Int32 = pivot.PivotFormatConditions.Add()
Dim pfc As PivotFormatCondition = pivot.PivotFormatConditions(formatIndex)
Dim fcc As FormatConditionCollection = pfc.FormatConditions
fcc.AddArea(pivot.DataBodyRange)
Dim idx As Int32 = fcc.AddCondition(FormatConditionType.CellValue)
Dim fc As FormatCondition = fcc(idx)
fc.Formula1 = "100"
fc.Operator = OperatorType.GreaterOrEqual
fc.Style.BackgroundColor = Color.Red

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Siehe auch

* namensraum [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
