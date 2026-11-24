---
title: "Klasse PivotTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotTable Klasse. Zusammenfassende Beschreibung für PivotTable"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

Zusammenfassende Beschreibung für die PivotTable.

```csharp
public class PivotTable : IDisposable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AllowMultipleFiltersPerField](../../aspose.cells.pivot/pivottable/allowmultiplefiltersperfield/) { get; set; } | Gibt einen booleschen Wert an, der angibt, ob die Felder einer PivotTable mehrere Filter haben können. |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription/) { get; set; } | Liest die Beschreibung des Alternativtexts. |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle/) { get; set; } | Liest und setzt den Titel des Alternativtexts. |
| [AutofitColumnWidthOnUpdate](../../aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/) { get; set; } | Gibt an, ob die Spaltenbreite bei einer Aktualisierung automatisch angepasst werden soll |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype/) { get; set; } | Liest und setzt den automatischen Formattyp der PivotTable. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields/) { get; } | Gibt alle Basis-Pivot-Felder in der PivotTable zurück. |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields/) { get; } | Gibt ein PivotFields-Objekt zurück, das derzeit als Spaltenfelder angezeigt wird. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand/) { get; set; } | (**Obsolete.**) Gibt an, ob der PivotTable-Bericht Gesamtsummen für Spalten anzeigt. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption/) { get; set; } | Liest und setzt die benutzerdefinierte Beschriftung der Spaltenüberschrift der PivotTable. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange/) { get; } | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Spaltenbereich im PivotTable-Bericht enthält. Schreibgeschützt. |
| [ConditionalFormats](../../aspose.cells.pivot/pivottable/conditionalformats/) { get; } | Liest die bedingten Formate der Pivot-Tabelle. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort/) { get; set; } | Gibt an, ob die integrierte benutzerdefinierte Liste beim Sortieren von Daten berücksichtigt wird. |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange/) { get; } | Gibt ein [`CellArea`](../../aspose.cells/cellarea/)‑Objekt zurück, das den Bereich darstellt, der den Datenbereich in der Liste zwischen der Kopfzeilenzeile und der Einfügezeile enthält. Nur lesbar. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield/) { get; } | (**Obsolete.**) Gibt ein [`PivotField`](../pivotfield/)‑Objekt zurück, das alle Datenfelder in einer PivotTable darstellt. Nur lesbar. Es wird nur erstellt, wenn im Datenbereich mindestens zwei Datenfelder vorhanden sind. Standardmäßig befindet es sich im Zeilenbereich. Sie können es mit der Methode PivotTable.AddFieldToArea() in den Zeilen‑/Spaltenbereich ziehen. |
| [DataFieldHeaderName](../../aspose.cells.pivot/pivottable/datafieldheadername/) { get; set; } | Liest und schreibt den Namen der Feldüberschrift des Wertebereichs in der PivotTable. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields/) { get; } | Gibt eine [`PivotFieldCollection`](../pivotfieldcollection/) zurück, die alle Datenfelder in einer PivotTable darstellt. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource/) { get; set; } | Liest und schreibt die Datenquelle der PivotTable. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring/) { get; set; } | Gibt an, ob der PivotTable-Bericht in Zellen, die Fehler enthalten, einen benutzerdefinierten Text anzeigt. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems/) { get; set; } | Gibt an, ob Elemente in den Zeilen‑ und Spaltenbereichen sichtbar sind, wenn der Datenbereich der PivotTable leer ist. Der Standardwert ist true. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring/) { get; set; } | Gibt an, ob der PivotTable-Bericht einen benutzerdefinierten Text anzeigt, wenn der Wert null ist. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting/) { get; set; } | Gibt einen booleschen Wert an, der festlegt, ob der Benutzer die Zellen im Datenbereich der PivotTable bearbeiten darf. Der Standardwert ist false. |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown/) { get; set; } | Gibt an, ob Drilldown aktiviert ist. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog/) { get; set; } | Gibt an, ob das Dialogfeld PivotTable‑Feld verfügbar ist, wenn der Benutzer das PivotTable‑Feld doppelt anklickt. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist/) { get; set; } | Gibt an, ob die Feldliste für die PivotTable in der Excel‑Ansicht verfügbar ist. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard/) { get; set; } | Gibt an, ob der PivotTable‑Assistent verfügbar ist. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring/) { get; set; } | Liest den Text, der in Zellen mit Fehlern angezeigt wird, wenn die Eigenschaft DisplayErrorString true ist. Der Standardwert ist ein leerer String. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource/) { get; } | (**Obsolete.**) Gibt die externe Verbindungsdatenquelle zurück. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending/) { get; set; } | Gibt an, ob Felder in der PivotTable in der Feldliste in einer nicht‑Standardreihenfolge sortiert sind. |
| [FilterArea](../../aspose.cells.pivot/pivottable/filterarea/) { get; } | Liest den Bereich der Filterregion. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname/) { get; set; } | Gibt die Bezeichnung zurück, die in der Überschrift der Gesamtsumme‑Spalte oder -Zeile angezeigt wird. Der Standardwert ist der String "Grand Total". |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows/) { get; set; } | (**Obsolete.**) Gibt an, ob leere Zeilen hinzugefügt werden sollen. Diese Eigenschaft gilt nur für PivotTable‑Autoformat‑Typen, die leere Zeilen benötigen. |
| [Indent](../../aspose.cells.pivot/pivottable/indent/) { get; set; } | Gibt die Einrückungssteigerung für die kompakte Achse an und kann verwendet werden, um das Berichtslayout auf kompakte Form einzustellen. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat/) { get; set; } | Gibt an, ob der PivotTable-Bericht automatisch formatiert wird. Kontrollkästchen "autoformat table", das in den PivotTable‑Optionen für Excel 2003 vorhanden ist. |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible/) { get; set; } | Gibt an, ob die PivotTable bei der Aktualisierung mit Excel 2003 kompatibel ist. Ist der Wert true, muss ein String höchstens 255 Zeichen lang sein; überschreitet er diese Länge, wird er abgeschnitten. Ist der Wert false, gilt diese Beschränkung nicht. Der Standardwert ist true. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones/) { get; set; } | Gibt an, ob der PivotTable-Bericht das klassische PivotTable‑Layout anzeigt (ermöglicht das Ziehen von Feldern im Raster). |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters/) { get; set; } | (**Obsolete.**) Gibt einen booleschen Wert an, der festlegt, ob die Felder einer PivotTable mehrere Filter gleichzeitig haben können. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected/) { get; set; } | Gibt an, ob diese PivotTable ausgewählt ist. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles/) { get; set; } | (**Obsolete.**) Gibt an, ob PivotItem-Namen oben auf jeder gedruckten Seite wiederholt werden sollen. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate/) { get; set; } | Gibt an, ob der PivotTable-Bericht nur auf Anforderung des Benutzers neu berechnet wird. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels/) { get; set; } | Liest oder legt fest, ob Zeilen-/Spaltenfeldbeschriftungen, die mehrere Zellen umfassen, zusammengeführt werden. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit/) { get; set; } | (**Obsolete.**) Gibt einen booleschen Wert an, der festlegt, ob die Felder einer PivotTable mehrere Filter gleichzeitig haben können. |
| [Name](../../aspose.cells.pivot/pivottable/name/) { get; set; } | Liest den Namen der PivotTable |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring/) { get; set; } | Liest die Zeichenkette, die in Zellen angezeigt wird, die Nullwerte enthalten, wenn die Eigenschaft DisplayNullString wahr ist. Der Standardwert ist eine leere Zeichenkette. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder/) { get; set; } | Liest und legt die Reihenfolge fest, in der Seitenfelder zum Layout des PivotTable-Berichts hinzugefügt werden. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields/) { get; } | Gibt eine [`PivotFieldCollection`](../pivotfieldcollection/) zurück, die derzeit als Seitenfelder angezeigt werden. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount/) { get; set; } | Liest die Anzahl der Seitenfelder in jeder Spalte oder Zeile im PivotTable-Bericht. |
| [PivotCache](../../aspose.cells.pivot/pivottable/pivotcache/) { get; } | Liest die Datenquelle. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters/) { get; } | Gibt alle Filter in der PivotTable zurück. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions/) { get; } | (**Obsolete.**) Liest die Formatbedingungen der PivotTable. |
| [PivotFormats](../../aspose.cells.pivot/pivottable/pivotformats/) { get; } | Liest alle Zellformate, die auf diese PivotTable angewendet werden. |
| [PivotTableStyle](../../aspose.cells.pivot/pivottable/pivottablestyle/) { get; set; } | Liest die TableStyle-Einstellungen dieser PivotTable. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename/) { get; set; } | Liest oder legt den Stilnamen der PivotTable fest. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype/) { get; set; } | Liest und legt den integrierten PivotTable-Stil fest. |
| [PreserveCellFormattingOnUpdate](../../aspose.cells.pivot/pivottable/preservecellformattingonupdate/) { get; set; } | Gibt an, ob die Zellformatierung ([`PivotTableFormat`](../pivottableformat/)) beibehalten werden soll, wenn die PivotTable aktualisiert oder neu berechnet wird. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting/) { get; set; } | (**Obsolete.**) Gibt an, ob die Zellformatierung ([`PivotTableFormat`](../pivottableformat/)) beibehalten wird, wenn die PivotTable aktualisiert oder neu berechnet wird. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill/) { get; set; } | Gibt einen booleschen Wert an, der angibt, ob Drill-Indikatoren gedruckt werden sollen. Druckt Expand-/Collapse‑Schaltflächen, wenn sie in der pivottable angezeigt werden. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles/) { get; set; } | Gibt an, ob die Drucktitel für das Arbeitsblatt basierend auf dem PivotTable-Bericht festgelegt werden. Der Standardwert ist false. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile/) { get; set; } | Gibt an, ob Daten beim Öffnen der Datei aktualisiert werden. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate/) { get; } | Liest das letzte Datum und die Uhrzeit, zu der die PivotTable aktualisiert wurde. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho/) { get; } | Liest den Namen des letzten Benutzers, der diese PivotTable aktualisiert hat |
| [RepeatItemsOnEachPrintedPage](../../aspose.cells.pivot/pivottable/repeatitemsoneachprintedpage/) { get; set; } | Gibt an, ob Beschriftungen von pivot item im Zeilenbereich auf jeder gedruckten Seite für Pivotfelder in Tabellenform wiederholt werden. |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields/) { get; } | Gibt eine [`PivotFieldCollection`](../pivotfieldcollection/) zurück, die derzeit als Zeilenfelder angezeigt werden. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand/) { get; set; } | (**Veraltet.**) Gibt an, ob Gesamtsummen für Zeilen dieser Pivot-Tabelle angezeigt werden sollen. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption/) { get; set; } | Liest und schreibt die benutzerdefinierte Beschriftung des Zeilenkopfes in dieser PivotTable. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange/) { get; } | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Zeilenbereich im PivotTable-Bericht enthält. Nur lesbar. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata/) { get; set; } | Gibt an, ob Daten für den PivotTable-Bericht mit der Arbeitsmappe gespeichert werden. |
| [ShowColumnGrandTotals](../../aspose.cells.pivot/pivottable/showcolumngrandtotals/) { get; set; } | Gibt an, ob Gesamtsummen für Spalten dieser Pivot-Tabelle angezeigt werden sollen. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips/) { get; set; } | Gibt an, ob Tooltips für PivotTable-Datenzellen angezeigt werden sollen. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill/) { get; set; } | Liest und schreibt, ob Expand/Collapse-Schaltflächen angezeigt werden. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol/) { get; set; } | Gibt an, ob leere Spalten in die Tabelle aufgenommen werden sollen |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow/) { get; set; } | Gibt an, ob leere Zeilen in die Tabelle aufgenommen werden sollen. |
| [ShowHeaders](../../aspose.cells.pivot/pivottable/showheaders/) { get; set; } | Ob Feldbeschriftungen und Pivot-Feldbeschriftungen auf der Zeilenachse und der Spaltenachse in der PivotTable-Ansicht angezeigt werden sollen. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips/) { get; set; } | Gibt einen booleschen Wert an, der festlegt, ob Member-Property-Informationen aus PivotTable-Tooltips weggelassen werden sollen. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader/) { get; set; } | Gibt an, ob die Spaltenüberschrift in der Pivot-Tabelle den Stil erhalten soll. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes/) { get; set; } | Gibt an, ob Streifenformatierung für die Spalte angewendet wird. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn/) { get; set; } | Gibt an, ob die Spaltenformatierung angewendet wird. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader/) { get; set; } | Gibt an, ob die Zeilenüberschrift in der Pivot-Tabelle den Stil erhalten soll. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes/) { get; set; } | Gibt an, ob Zeilenstreifenformatierung angewendet wird. |
| [ShowRowGrandTotals](../../aspose.cells.pivot/pivottable/showrowgrandtotals/) { get; set; } | Gibt an, ob Gesamtsummen für Zeilen der Pivot-Tabelle angezeigt werden sollen. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption/) { get; set; } | (**Veraltet.**) Gibt an, ob die Zeilenkopfzeilenbeschriftung im PivotTable-Bericht angezeigt wird Gibt an, ob Feldbeschriftungen und Filter-Dropdowns angezeigt werden |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow/) { get; set; } | Gibt an, ob die Wertezeile angezeigt wird. |
| [SourceType](../../aspose.cells.pivot/pivottable/sourcetype/) { get; } | Liest den Typ der Datenquelle der Pivot-Tabelle. |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems/) { get; set; } | Gibt an, ob ausgeblendete Seitenfeld-Elemente im PivotTable-Bericht in Zeilen- und Spalten-Teilsummen, Blocksummen und Gesamtsummen einbezogen werden. Der Standardwert ist False. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1/) { get; } | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den gesamten PivotTable-Bericht enthält, jedoch keine Seitenfelder einschließt. Nur lesbar. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2/) { get; } | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den gesamten PivotTable-Bericht enthält, einschließlich Seitenfelder. Nur lesbar. |
| [Tag](../../aspose.cells.pivot/pivottable/tag/) { get; set; } | Liest und schreibt eine benutzerdefinierte Zeichenkette, die mit dieser PivotTable-Ansicht verknüpft ist. |
| [TopRightArea](../../aspose.cells.pivot/pivottable/toprightarea/) { get; } | Stellt den leeren Bereich oben rechts der PivotTable dar (oben links für RTL-Blätter). |
| [ValuesField](../../aspose.cells.pivot/pivottable/valuesfield/) { get; } | Ruft ein [`PivotField`](../pivotfield/) Objekt ab, das alle Datenfelder in einer PivotTable darstellt. Nur lesbar. Es wird nur erstellt, wenn im Datenbereich zwei oder mehr Datenfelder vorhanden sind. Standardmäßig befindet es sich im Zeilenbereich. Sie können es mit der Methode PivotTable.AddFieldToArea() in den Zeilen‑/Spaltenbereich ziehen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield)(string, string) | Fügt ein berechnetes Feld zum PivotField hinzu und zieht es in den Datenbereich. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield_1)(string, string, bool) | Fügt ein berechnetes Feld zum PivotField hinzu. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_1)(PivotFieldType, int) | Fügt das Feld dem spezifischen Bereich hinzu. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea)(PivotFieldType, PivotField) | Fügt das Feld dem spezifischen Bereich hinzu. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_2)(PivotFieldType, string) | Fügt das Feld dem spezifischen Bereich hinzu. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata_1)() | Berechnet die Daten der PivotTable in Zellen. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata)(PivotTableCalculateOption) | Berechnet die PivotTable mit Optionen. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange/)() | Berechnet den Bereich der PivotTable. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource/)(string[]) | Ändert die Datenquelle der PivotTable. |
| [ClearAll](../../aspose.cells.pivot/pivottable/clearall/)() | Entfernt alle Felder aus den Bereichen. |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata/)() | Löscht Daten und Formatierung der PivotTable‑Ansicht. |
| [ClearFilters](../../aspose.cells.pivot/pivottable/clearfilters/)() | Löscht alle Filter dieser PivotTable. |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle/)(PivotTable) | Kopiert benannten Stil von einer anderen PivotTable. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose/)() | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [ExportViewToJson](../../aspose.cells.pivot/pivottable/exportviewtojson/)(PivotViewToJsonOptions) | Exportiert die Pivot‑Ansicht als JSON. |
| [Fields](../../aspose.cells.pivot/pivottable/fields/)(PivotFieldType) | (**Veraltet.**) Ruft die spezifischen Felder nach Feldtyp ab. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format)(CellArea, Style) | Formatiert den ausgewählten Bereich der PivotTable. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_1)(PivotArea, Style) | Formatiert den ausgewählten Bereich der PivotTable. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_2)(int, int, Style) | Formatiert die Zelle im PivotTable‑Bereich |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall/)(Style) | Formatiert alle Zellen im PivotTable‑Bereich |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow/)(int, Style) | Formatiert die Zeilendaten im PivotTable‑Bereich |
| [GetButtonArea](../../aspose.cells.pivot/pivottable/getbuttonarea/)(PivotFieldType) | Ruft den Bereich ab, der den Feld‑Button enthält. |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname/)(string) | Ruft das [`Cell`](../../aspose.cells/cell/) Objekt anhand des Anzeigennamens von PivotField ab. |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren/)() | (**Veraltet.**) Ruft die untergeordneten PivotTables ab, die diese PivotTable‑Daten als Datenquelle verwenden. |
| [GetDependentPivotTables](../../aspose.cells.pivot/pivottable/getdependentpivottables/)() | Ruft alle `PivotTable`s ab, die diese PivotTable als Datenquelle verwenden. |
| [GetFields](../../aspose.cells.pivot/pivottable/getfields/)(PivotFieldType) | Ruft die spezifische PivotField‑Liste nach Region ab. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks/)() | (**Veraltet.**) Ruft die Zeilenindexliste der PivotTable für horizontale Seitenumbrüche ab |
| [GetHorizontalPageBreaks](../../aspose.cells.pivot/pivottable/gethorizontalpagebreaks/)() | Ruft horizontale Seitenumbrüche dieser PivotTable ab. |
| [GetNamesOfSourceDataConnections](../../aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/)() | Ruft die Namen externer Datenquellenverbindungen ab. |
| [GetPivotTablesWithSamePivotCache](../../aspose.cells.pivot/pivottable/getpivottableswithsamepivotcache/)() | Ermittelt alle Pivot-Tabellen mit demselben Pivot-Cache. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource)() | Erhalte die Datenquelle dieser Pivot-Tabelle. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource_1)(bool) | Erhalte die Datenquelle dieser Pivot-Tabelle. |
| [GetSourceDataConnections](../../aspose.cells.pivot/pivottable/getsourcedataconnections/)() | Ermittelt die Datenquellen externer Verbindungen. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move_1)(string) | (**Obsolete.**) Verschiebt die PivotTable an eine andere Position im Arbeitsblatt. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move)(int, int) | (**Obsolete.**) Verschiebt die PivotTable an eine andere Position im Arbeitsblatt. |
| [MoveItem](../../aspose.cells.pivot/pivottable/moveitem/)(PivotFieldType, string[], bool, int) | Verschiebe ein Element nach oben oder unten. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_2)(string) | Verschiebt die PivotTable an eine andere Position im Arbeitsblatt. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto)(int, int) | Verschiebt die PivotTable an eine andere Position im Arbeitsblatt. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_1)(int, int, int) | Verschiebt die PivotTable an eine andere Position im Arbeitsblatt. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh)() | Aktualisiere [`PivotCache`](./pivotcache/) aus der Datenquelle und berechne Daten und Stil für die Pivot-Ansicht. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh_1)(PivotTableRefreshOption) | Aktualisiere [`PivotCache`](./pivotcache/) aus der Datenquelle und berechne Daten und Stil für die Pivot-Ansicht. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata)() | (**Obsolete.**) Aktualisiert Daten aus seiner Datenquelle zum Pivot-Cache. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata_1)(PivotTableRefreshOption) | (**Obsolete.**) Aktualisiert die Daten und Einstellungen der PivotTable aus ihrer Datenquelle mit Optionen. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_1)(PivotFieldType, int) | Entfernt ein Feld aus einem bestimmten Pivot-Bereich. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield)(PivotFieldType, PivotField) | Entferne Feld aus einem bestimmten Feldbereich |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_2)(PivotFieldType, string) | Entfernt ein Feld aus einem bestimmten Feldbereich |
| [SelectArea](../../aspose.cells.pivot/pivottable/selectarea/)(CellArea) | Wähle einen Bereich der Pivot-Tabellenansicht aus. |
| [ShowDetail](../../aspose.cells.pivot/pivottable/showdetail/)(int, int, bool, int, int) | Zeige die Details eines Elements im Datenbereich in einer neuen Tabelle an. |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform/)() | Gestaltet die PivotTable-Ansicht in kompakter Form. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform/)() | Gestaltet die PivotTable in Gliederungsform. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform/)() | Gestaltet die PivotTable in Tabellenform. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage/)(PivotField) | Zeige alle Berichtfilterseiten basierend auf PivotField an, wobei das PivotField in den PageFields liegen muss. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex/)(int) | Zeige alle Berichtfilterseiten basierend auf dem Positionsindex in den PageFields an. |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname/)(string) | Zeige alle Berichtfilterseiten basierend auf dem Namen des PivotField an, wobei das PivotField in den PageFields liegen muss. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotTableDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Beispieldaten festlegen
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";

            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;

            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;

            // Pivot-Tabelle erstellen
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];

            // Felder hinzufügen
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Gestalte die Pivot-Tabelle
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Zeilenfeld anpassen
            PivotField rowField = pivot.RowFields[0];
            rowField.DisplayName = "Fruit Category";

            // Aktualisieren und Daten berechnen
            pivot.RefreshData();
            pivot.CalculateData();

            // Speichere die Arbeitsmappe
            book.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


