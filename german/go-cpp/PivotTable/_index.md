---
title: "PivotTable Klasse"
linktitle: "PivotTable"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PivotTable Klasse. Kapselt das Objekt, das eine PivotTable in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/pivottable/
---

## PivotTable class

Zusammenfassende Beschreibung für PivotTable.

```go

type PivotTable struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [Dispose](./dispose/) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [GetPivotCache](./getpivotcache/) | Liefert die Datenquelle. |
| [IsExcel2003Compatible](./isexcel2003compatible/) | Gibt an, ob die PivotTable beim Aktualisieren mit Excel2003 kompatibel ist; wenn true, muss ein String höchstens 255 Zeichen lang sein, sodass ein längerer String abgeschnitten wird. Wenn false, gilt die genannte Beschränkung nicht. Der Standardwert ist true. |
| [SetIsExcel2003Compatible](./setisexcel2003compatible/) | Gibt an, ob die PivotTable beim Aktualisieren mit Excel2003 kompatibel ist; wenn true, muss ein String höchstens 255 Zeichen lang sein, sodass ein längerer String abgeschnitten wird. Wenn false, gilt die genannte Beschränkung nicht. Der Standardwert ist true. |
| [GetRefreshedByWho](./getrefreshedbywho/) | Liefert den Namen des letzten Benutzers, der diese PivotTable aktualisiert hat |
| [GetRefreshDate](./getrefreshdate/) | Liefert das letzte Datum und die Uhrzeit, zu der die PivotTable aktualisiert wurde. |
| [GetPivotTableStyle](./getpivottablestyle/) | Liefert die TableStyle-Einstellungen dieser PivotTable. |
| [SetPivotTableStyle](./setpivottablestyle/) | Liefert die TableStyle-Einstellungen dieser PivotTable. |
| [GetPivotTableStyleName](./getpivottablestylename/) | Liefert oder setzt den Stilnamen der PivotTable. |
| [SetPivotTableStyleName](./setpivottablestylename/) | Liefert oder setzt den Stilnamen der PivotTable. |
| [GetPivotTableStyleType](./getpivottablestyletype/) | Liefert und setzt den integrierten PivotTable-Stil. |
| [SetPivotTableStyleType](./setpivottablestyletype/) | Liefert und setzt den integrierten PivotTable-Stil. |
| [CopyStyle](./copystyle/) | Kopiert den benannten Stil von einer anderen PivotTable. |
| [ShowReportFilterPage](./showreportfilterpage/) | Zeigt alle Berichtfilterseiten basierend auf PivotField an; das PivotField muss sich in den PageFields befinden. |
| [ShowReportFilterPageByName](./showreportfilterpagebyname/) | Zeigt alle Berichtfilterseiten basierend auf dem Namen von PivotField an; das PivotField muss sich in den PageFields befinden. |
| [ShowReportFilterPageByIndex](./showreportfilterpagebyindex/) | Zeigt alle Berichtfilterseiten basierend auf dem Positionsindex in den PageFields an. |
| [RemoveField_PivotFieldType_String](./removefield_pivotfieldtype_string/) | Entfernt ein Feld aus einem bestimmten Feldbereich |
| [RemoveField_PivotFieldType_Int](./removefield_pivotfieldtype_int/) | Entfernt ein Feld aus einer bestimmten Pivot-Region. |
| [RemoveField_PivotFieldType_PivotField](./removefield_pivotfieldtype_pivotfield/) | Feld aus einem bestimmten Feldbereich entfernen |
| [AddFieldToArea_PivotFieldType_String](./addfieldtoarea_pivotfieldtype_string/) | Fügt das Feld dem bestimmten Bereich hinzu. |
| [AddFieldToArea_PivotFieldType_Int](./addfieldtoarea_pivotfieldtype_int/) | Fügt das Feld dem bestimmten Bereich hinzu. |
| [AddFieldToArea_PivotFieldType_PivotField](./addfieldtoarea_pivotfieldtype_pivotfield/) | Fügt das Feld dem bestimmten Bereich hinzu. |
| [AddCalculatedField_String_String_Bool](./addcalculatedfield_string_string_bool/) | Fügt ein berechnetes Feld zum PivotField hinzu. |
| [AddCalculatedField_String_String](./addcalculatedfield_string_string/) | Fügt ein berechnetes Feld zum PivotField hinzu und zieht es in den Datenbereich. |
| [GetFields](./getfields/) | Liefert die spezifische PivotField-Liste nach Region. |
| [GetColumnFields](./getcolumnfields/) | Gibt ein PivotFields-Objekt zurück, das derzeit als Spaltenfelder angezeigt wird. |
| [GetRowFields](./getrowfields/) | Gibt ein PivotFields-Objekt zurück, das derzeit als Zeilenfelder angezeigt wird. |
| [GetPageFields](./getpagefields/) | Gibt ein PivotFields-Objekt zurück, das derzeit als Seitenfelder angezeigt wird. |
| [GetDataFields](./getdatafields/) | Liefert ein PivotField-Objekt, das alle Datenfelder in einer PivotTable darstellt. Nur lesbar. Es wird nur initialisiert, wenn es zwei oder mehr Datenfelder in den DataPiovtFiels gibt. Es wird ausschließlich verwendet, um DataPivotField zum Zeilen‑/Spaltenbereich der PivotTable hinzuzufügen. Standardmäßig ist es im Zeilenbereich. |
| [GetValuesField](./getvaluesfield/) | Liefert ein PivotField-Objekt, das alle Datenfelder in einer PivotTable darstellt. Schreibgeschützt. Es wird nur erstellt, wenn im Datenbereich zwei oder mehr Datenfelder vorhanden sind. Standardmäßig befindet es sich im Zeilenbereich. Sie können es mit der Methode PivotTable.AddFieldToArea() in den Zeilen‑/Spaltenbereich ziehen. |
| [GetBaseFields](./getbasefields/) | Gibt alle Basis‑Pivot‑Felder in der PivotTable zurück. |
| [GetPivotFilters](./getpivotfilters/) | Gibt alle Filter von Pivot‑Feldern in der PivotTable zurück. |
| [GetButtonArea](./getbuttonarea/) | Liefert den Bereich, der die Feldschaltfläche enthält. |
| [GetTopRightArea](./gettoprightarea/) | Stellt den leeren Bereich oben rechts in der PivotTable dar (oben links für RTL‑Blätter). |
| [GetFilterArea](./getfilterarea/) | Liefert den Bereich der Filterregion. |
| [GetColumnRange](./getcolumnrange/) | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Spaltenbereich im PivotTable-Bericht enthält. Schreibgeschützt. |
| [GetRowRange](./getrowrange/) | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der den Zeilenbereich im PivotTable-Bericht enthält. Schreibgeschützt. |
| [GetDataBodyRange](./getdatabodyrange/) | Gibt ein CellArea-Objekt zurück, das den Bereich darstellt, der die Datenfläche in der Liste zwischen der Kopfzeile und der Einfügezeile enthält. Schreibgeschützt. |
| [GetTableRange1](./gettablerange1/) | Gibt ein CellArea-Objekt zurück, das den Bereich enthält, der den gesamten PivotTable-Bericht umfasst, jedoch keine Seitenfelder. Schreibgeschützt. |
| [GetTableRange2](./gettablerange2/) | Gibt ein CellArea-Objekt zurück, das den Bereich enthält, der den gesamten PivotTable-Bericht umfasst, einschließlich Seitenfelder. Schreibgeschützt. |
| [MoveTo_Int_Int](./moveto_int_int/) | Verschiebt die PivotTable an einen anderen Ort im Arbeitsblatt. |
| [MoveTo_Int_Int_Int](./moveto_int_int_int/) | Verschiebt die PivotTable an einen anderen Ort im Arbeitsblatt. |
| [MoveTo_String](./moveto_string/) | Verschiebt die PivotTable an einen anderen Ort im Arbeitsblatt. |
| [IsGridDropZones](./isgriddropzones/) | Gibt an, ob der PivotTable-Bericht das klassische PivotTable‑Layout anzeigt (ermöglicht das Ziehen von Feldern im Raster). |
| [SetIsGridDropZones](./setisgriddropzones/) | Gibt an, ob der PivotTable-Bericht das klassische PivotTable‑Layout anzeigt (ermöglicht das Ziehen von Feldern im Raster). |
| [GetShowColumnGrandTotals](./getshowcolumngrandtotals/) | Gibt an, ob Gesamtsummen für die Spalten dieser PivotTable angezeigt werden sollen. |
| [SetShowColumnGrandTotals](./setshowcolumngrandtotals/) | Gibt an, ob Gesamtsummen für die Spalten dieser PivotTable angezeigt werden sollen. |
| [GetShowRowGrandTotals](./getshowrowgrandtotals/) | Gibt an, ob Gesamtsummen für die Zeilen der PivotTable angezeigt werden sollen. |
| [SetShowRowGrandTotals](./setshowrowgrandtotals/) | Gibt an, ob Gesamtsummen für die Zeilen der PivotTable angezeigt werden sollen. |
| [GetDisplayNullString](./getdisplaynullstring/) | Gibt an, ob der PivotTable-Bericht einen benutzerdefinierten Text anzeigt, wenn der Wert null ist. |
| [SetDisplayNullString](./setdisplaynullstring/) | Gibt an, ob der PivotTable-Bericht einen benutzerdefinierten Text anzeigt, wenn der Wert null ist. |
| [GetNullString](./getnullstring/) | Liefert den Text, der in Zellen mit Nullwerten angezeigt wird, wenn die Eigenschaft DisplayNullString wahr ist. Der Standardwert ist ein leerer String. |
| [SetNullString](./setnullstring/) | Liefert den Text, der in Zellen mit Nullwerten angezeigt wird, wenn die Eigenschaft DisplayNullString wahr ist. Der Standardwert ist ein leerer String. |
| [GetDisplayErrorString](./getdisplayerrorstring/) | Gibt an, ob der PivotTable-Bericht einen benutzerdefinierten Text in Zellen mit Fehlern anzeigt. |
| [SetDisplayErrorString](./setdisplayerrorstring/) | Gibt an, ob der PivotTable-Bericht einen benutzerdefinierten Text in Zellen mit Fehlern anzeigt. |
| [GetDataFieldHeaderName](./getdatafieldheadername/) | Liest und schreibt den Namen der Feldüberschrift im Wertebereich der PivotTable. |
| [SetDataFieldHeaderName](./setdatafieldheadername/) | Liest und schreibt den Namen der Feldüberschrift im Wertebereich der PivotTable. |
| [GetErrorString](./geterrorstring/) | Liefert den Text, der in Zellen mit Fehlern angezeigt wird, wenn die Eigenschaft DisplayErrorString wahr ist. Der Standardwert ist ein leerer String. |
| [SetErrorString](./seterrorstring/) | Liefert den Text, der in Zellen mit Fehlern angezeigt wird, wenn die Eigenschaft DisplayErrorString wahr ist. Der Standardwert ist ein leerer String. |
| [IsAutoFormat](./isautoformat/) | Gibt an, ob der PivotTable-Bericht automatisch formatiert wird. Kontrollkästchen \"autoformat table\", das in den PivotTable-Optionen für Excel 2003 zu finden ist. |
| [SetIsAutoFormat](./setisautoformat/) | Gibt an, ob der PivotTable-Bericht automatisch formatiert wird. Kontrollkästchen \"autoformat table\", das in den PivotTable-Optionen für Excel 2003 zu finden ist. |
| [GetAutofitColumnWidthOnUpdate](./getautofitcolumnwidthonupdate/) | Gibt an, ob die Spaltenbreite bei einer Aktualisierung automatisch angepasst wird. |
| [SetAutofitColumnWidthOnUpdate](./setautofitcolumnwidthonupdate/) | Gibt an, ob die Spaltenbreite bei einer Aktualisierung automatisch angepasst wird. |
| [GetAutoFormatType](./getautoformattype/) | Liest und schreibt den automatischen Formattyp der PivotTable. |
| [SetAutoFormatType](./setautoformattype/) | Liest und schreibt den automatischen Formattyp der PivotTable. |
| [GetMergeLabels](./getmergelabels/) | Gibt an, ob Zeilen‑ oder Spaltentitel, die mehrere Zellen umfassen, zu einer einzelnen Zelle zusammengeführt werden sollen. |
| [SetMergeLabels](./setmergelabels/) | Gibt an, ob Zeilen‑ oder Spaltentitel, die mehrere Zellen umfassen, zu einer einzelnen Zelle zusammengeführt werden sollen. |
| [GetPreserveCellFormattingOnUpdate](./getpreservecellformattingonupdate/) | Gibt an, ob die Zellformatierung (PivotTableFormat) beim Aktualisieren oder Neuberechnen der PivotTable beibehalten werden soll. |
| [SetPreserveCellFormattingOnUpdate](./setpreservecellformattingonupdate/) | Gibt an, ob die Zellformatierung (PivotTableFormat) beim Aktualisieren oder Neuberechnen der PivotTable beibehalten werden soll. |
| [GetShowDrill](./getshowdrill/) | Liest und setzt, ob Expand/Collapse‑Schaltflächen angezeigt werden. |
| [SetShowDrill](./setshowdrill/) | Liest und setzt, ob Expand/Collapse‑Schaltflächen angezeigt werden. |
| [GetEnableDrilldown](./getenabledrilldown/) | Gibt an, ob Drilldown aktiviert ist. |
| [SetEnableDrilldown](./setenabledrilldown/) | Gibt an, ob Drilldown aktiviert ist. |
| [GetEnableFieldDialog](./getenablefielddialog/) | Gibt an, ob das Dialogfeld PivotTable Field verfügbar ist, wenn der Benutzer das PivotTable‑Feld doppelklickt. |
| [SetEnableFieldDialog](./setenablefielddialog/) | Gibt an, ob das Dialogfeld PivotTable Field verfügbar ist, wenn der Benutzer das PivotTable‑Feld doppelklickt. |
| [GetEnableFieldList](./getenablefieldlist/) | Gibt an, ob die Feldliste für die PivotTable in der Excel‑Ansicht verfügbar ist. |
| [SetEnableFieldList](./setenablefieldlist/) | Gibt an, ob die Feldliste für die PivotTable in der Excel‑Ansicht verfügbar ist. |
| [GetEnableWizard](./getenablewizard/) | Gibt an, ob der PivotTable‑Assistent verfügbar ist. |
| [SetEnableWizard](./setenablewizard/) | Gibt an, ob der PivotTable‑Assistent verfügbar ist. |
| [GetSubtotalHiddenPageItems](./getsubtotalhiddenpageitems/) | Gibt an, ob versteckte Seitenfeld‑Elemente im PivotTable‑Bericht in Zeilen‑ und Spaltensummen, Blocksummen und Gesamtsummen einbezogen werden. Der Standardwert ist False. |
| [SetSubtotalHiddenPageItems](./setsubtotalhiddenpageitems/) | Gibt an, ob versteckte Seitenfeld‑Elemente im PivotTable‑Bericht in Zeilen‑ und Spaltensummen, Blocksummen und Gesamtsummen einbezogen werden. Der Standardwert ist False. |
| [GetGrandTotalName](./getgrandtotalname/) | Gibt die Beschriftung zurück, die in der Gesamtsumme‑Spalte oder -Zeilenüberschrift angezeigt wird. Der Standardwert ist die Zeichenkette "Grand Total". |
| [SetGrandTotalName](./setgrandtotalname/) | Gibt die Beschriftung zurück, die in der Gesamtsumme‑Spalte oder -Zeilenüberschrift angezeigt wird. Der Standardwert ist die Zeichenkette "Grand Total". |
| [GetManualUpdate](./getmanualupdate/) | Gibt an, ob der PivotTable‑Bericht nur auf Anforderung des Benutzers neu berechnet wird. |
| [SetManualUpdate](./setmanualupdate/) | Gibt an, ob der PivotTable‑Bericht nur auf Anforderung des Benutzers neu berechnet wird. |
| [GetAllowMultipleFiltersPerField](./getallowmultiplefiltersperfield/) | Gibt einen booleschen Wert an, der angibt, ob die Felder einer PivotTable mehrere Filter gleichzeitig haben können. |
| [SetAllowMultipleFiltersPerField](./setallowmultiplefiltersperfield/) | Gibt einen booleschen Wert an, der angibt, ob die Felder einer PivotTable mehrere Filter gleichzeitig haben können. |
| [GetEnableDataValueEditing](./getenabledatavalueediting/) | Gibt einen booleschen Wert an, der angibt, ob der Benutzer die Zellen im Datenbereich der PivotTable bearbeiten darf. Zellbearbeitung im Wertebereich aktivieren |
| [SetEnableDataValueEditing](./setenabledatavalueediting/) | Gibt einen booleschen Wert an, der angibt, ob der Benutzer die Zellen im Datenbereich der PivotTable bearbeiten darf. Zellbearbeitung im Wertebereich aktivieren |
| [GetShowDataTips](./getshowdatatips/) | Gibt an, ob Tooltips für PivotTable‑Datenzellen angezeigt werden sollen. |
| [SetShowDataTips](./setshowdatatips/) | Gibt an, ob Tooltips für PivotTable‑Datenzellen angezeigt werden sollen. |
| [GetShowMemberPropertyTips](./getshowmemberpropertytips/) | Gibt einen booleschen Wert an, der angibt, ob Mitgliedseigenschaftsinformationen aus PivotTable‑Tooltips weggelassen werden sollen. |
| [SetShowMemberPropertyTips](./setshowmemberpropertytips/) | Gibt einen booleschen Wert an, der angibt, ob Mitgliedseigenschaftsinformationen aus PivotTable‑Tooltips weggelassen werden sollen. |
| [GetShowValuesRow](./getshowvaluesrow/) | Gibt an, ob die Werte‑Zeile angezeigt wird. |
| [SetShowValuesRow](./setshowvaluesrow/) | Gibt an, ob die Werte‑Zeile angezeigt wird. |
| [GetShowEmptyCol](./getshowemptycol/) | Gibt an, ob leere Spalten in die Tabelle aufgenommen werden sollen |
| [SetShowEmptyCol](./setshowemptycol/) | Gibt an, ob leere Spalten in die Tabelle aufgenommen werden sollen |
| [GetShowEmptyRow](./getshowemptyrow/) | Gibt an, ob leere Zeilen in die Tabelle aufgenommen werden sollen. |
| [SetShowEmptyRow](./setshowemptyrow/) | Gibt an, ob leere Zeilen in die Tabelle aufgenommen werden sollen. |
| [GetFieldListSortAscending](./getfieldlistsortascending/) | Gibt an, ob Felder in der PivotTable in der Feldliste in einer nicht‑Standardreihenfolge sortiert sind. |
| [SetFieldListSortAscending](./setfieldlistsortascending/) | Gibt an, ob Felder in der PivotTable in der Feldliste in einer nicht‑Standardreihenfolge sortiert sind. |
| [GetPrintDrill](./getprintdrill/) | Gibt einen booleschen Wert an, der angibt, ob Drill‑Indikatoren gedruckt werden sollen. Expand/Collapse‑Schaltflächen beim Anzeigen in der PivotTable drucken. |
| [SetPrintDrill](./setprintdrill/) | Gibt einen booleschen Wert an, der angibt, ob Drill‑Indikatoren gedruckt werden sollen. Expand/Collapse‑Schaltflächen beim Anzeigen in der PivotTable drucken. |
| [GetAltTextTitle](./getalttexttitle/) | Liest und setzt den Titel des Alternativtexts. |
| [SetAltTextTitle](./setalttexttitle/) | Liest und setzt den Titel des Alternativtexts. |
| [GetAltTextDescription](./getalttextdescription/) | Liest die Beschreibung des Alternativtexts. |
| [SetAltTextDescription](./setalttextdescription/) | Liest die Beschreibung des Alternativtexts. |
| [GetName](./getname/) | Liest den Namen der PivotTable |
| [SetName](./setname/) | Liest den Namen der PivotTable |
| [GetColumnHeaderCaption](./getcolumnheadercaption/) | Liest und setzt die benutzerdefinierte Beschriftung des Spaltenkopfs der PivotTable. |
| [SetColumnHeaderCaption](./setcolumnheadercaption/) | Liest und setzt die benutzerdefinierte Beschriftung des Spaltenkopfs der PivotTable. |
| [GetIndent](./getindent/) | Gibt die Einrückungs­schrittweite für die kompakte Achse an und kann verwendet werden, um das Berichtslayout auf kompakte Form einzustellen. |
| [SetIndent](./setindent/) | Gibt die Einrückungs­schrittweite für die kompakte Achse an und kann verwendet werden, um das Berichtslayout auf kompakte Form einzustellen. |
| [GetRowHeaderCaption](./getrowheadercaption/) | Liest und setzt die benutzerdefinierte Beschriftung des Zeilenkopfs in dieser PivotTable. |
| [SetRowHeaderCaption](./setrowheadercaption/) | Liest und setzt die benutzerdefinierte Beschriftung des Zeilenkopfs in dieser PivotTable. |
| [GetShowHeaders](./getshowheaders/) | Ob Datenfeld‑Beschriftungen und Pivot‑Feld‑Beschriftungen auf der Zeilen‑ und Spaltenachse in der PivotTable‑Ansicht angezeigt werden sollen. |
| [SetShowHeaders](./setshowheaders/) | Ob Datenfeld‑Beschriftungen und Pivot‑Feld‑Beschriftungen auf der Zeilen‑ und Spaltenachse in der PivotTable‑Ansicht angezeigt werden sollen. |
| [GetCustomListSort](./getcustomlistsort/) | Gibt an, ob die integrierte benutzerdefinierte Liste beim Sortieren von Daten berücksichtigt werden soll |
| [SetCustomListSort](./setcustomlistsort/) | Gibt an, ob die integrierte benutzerdefinierte Liste beim Sortieren von Daten berücksichtigt werden soll |
| [GetConditionalFormats](./getconditionalformats/) | Liefert die bedingten Formate der Pivot-Tabelle. |
| [GetPageFieldOrder](./getpagefieldorder/) | Liefert und setzt die Reihenfolge, in der Seitenfelder zum Layout des PivotTable-Berichts hinzugefügt werden. |
| [SetPageFieldOrder](./setpagefieldorder/) | Liefert und setzt die Reihenfolge, in der Seitenfelder zum Layout des PivotTable-Berichts hinzugefügt werden. |
| [GetPageFieldWrapCount](./getpagefieldwrapcount/) | Liefert die Anzahl der Seitenfelder in jeder Spalte oder Zeile im PivotTable-Bericht. |
| [SetPageFieldWrapCount](./setpagefieldwrapcount/) | Liefert die Anzahl der Seitenfelder in jeder Spalte oder Zeile im PivotTable-Bericht. |
| [GetTag](./gettag/) | Liefert und setzt eine benutzerdefinierte Zeichenkette, die mit dieser PivotTable-Ansicht verknüpft ist. |
| [SetTag](./settag/) | Liefert und setzt eine benutzerdefinierte Zeichenkette, die mit dieser PivotTable-Ansicht verknüpft ist. |
| [GetSaveData](./getsavedata/) | Gibt an, ob Daten für den PivotTable-Bericht mit der Arbeitsmappe gespeichert werden. |
| [SetSaveData](./setsavedata/) | Gibt an, ob Daten für den PivotTable-Bericht mit der Arbeitsmappe gespeichert werden. |
| [GetRefreshDataOnOpeningFile](./getrefreshdataonopeningfile/) | Gibt an, ob Daten beim Öffnen der Datei aktualisiert werden. |
| [SetRefreshDataOnOpeningFile](./setrefreshdataonopeningfile/) | Gibt an, ob Daten beim Öffnen der Datei aktualisiert werden. |
| [GetSourceType](./getsourcetype/) | Liefert den Datentyp der Datenquelle der Pivot-Tabelle. |
| [GetSourceDataConnections](./getsourcedataconnections/) | Liefert die externen Verbindungsdatenquellen. |
| [GetNamesOfSourceDataConnections](./getnamesofsourcedataconnections/) | Liefert die Namen der externen Datenquellenverbindungen. |
| [GetDataSource](./getdatasource/) | Liefert und setzt die Datenquelle der Pivot-Tabelle. |
| [SetDataSource](./setdatasource/) | Liefert und setzt die Datenquelle der Pivot-Tabelle. |
| [ChangeDataSource](./changedatasource/) | Ändere die Datenquelle der Pivot-Tabelle. |
| [GetSource](./getsource/) | Liefere die Datenquelle dieser Pivot-Tabelle. |
| [GetSource_Bool](./getsource_bool/) | Liefere die Datenquelle dieser Pivot-Tabelle. |
| [Refresh](./refresh/) | Aktualisiere den PivotCache aus der Datenquelle und berechne Daten und Stil für die Pivot-Ansicht. |
| [CalculateData](./calculatedata/) | Berechnet die Daten der Pivot-Tabelle in Zellen. |
| [CalculateData_PivotTableCalculateOption](./calculatedata_pivottablecalculateoption/) | Berechnet die Pivot-Tabelle mit Optionen. |
| [GetPivotTablesWithSamePivotCache](./getpivottableswithsamepivotcache/) | Liefert alle Pivot-Tabellen mit demselben Pivot-Cache. |
| [ClearData](./cleardata/) | Löscht Daten und Formatierung der PivotTable-Ansicht. |
| [ClearFilters](./clearfilters/) | Löscht alle Filter dieser Pivot-Tabelle. |
| [ClearAll](./clearall/) | Entfernt alle Felder aus Regionen. |
| [CalculateRange](./calculaterange/) | Berechnet den Bereich der Pivot-Tabelle. |
| [FormatAll](./formatall/) | Formatiere alle Zellen im Pivot-Tabellenbereich |
| [FormatRow](./formatrow/) | Formatiere die Zeilendaten im Pivot-Tabellenbereich |
| [Format_PivotArea_Style](./format_pivotarea_style/) | Formatiert den ausgewählten Bereich der PivotTable. |
| [Format_CellArea_Style](./format_cellarea_style/) | Formatiert den ausgewählten Bereich der PivotTable. |
| [Format_Int_Int_Style](./format_int_int_style/) | Formatiert die Zelle im Pivot-Tabellenbereich |
| [SelectArea](./selectarea/) | Wähle einen Bereich der Pivot-Tabellenansicht aus. |
| [ShowDetail](./showdetail/) | Zeige die Details eines Elements im Datenbereich in einer neuen Tabelle. |
| [GetPivotFormats](./getpivotformats/) | Ermittelt alle auf die PivotTable angewendeten Formate. |
| [GetRepeatItemsOnEachPrintedPage](./getrepeatitemsoneachprintedpage/) | Gibt an, ob Beschriftungen des Pivot-Elements im Zeilenbereich auf jeder gedruckten Seite für Pivot-Felder in Tabellenform wiederholt werden. |
| [SetRepeatItemsOnEachPrintedPage](./setrepeatitemsoneachprintedpage/) | Gibt an, ob Beschriftungen des Pivot-Elements im Zeilenbereich auf jeder gedruckten Seite für Pivot-Felder in Tabellenform wiederholt werden. |
| [GetPrintTitles](./getprinttitles/) | Gibt an, ob die Drucktitel für das Arbeitsblatt basierend auf dem PivotTable-Bericht festgelegt sind. Der Standardwert ist false. |
| [SetPrintTitles](./setprinttitles/) | Gibt an, ob die Drucktitel für das Arbeitsblatt basierend auf dem PivotTable-Bericht festgelegt sind. Der Standardwert ist false. |
| [GetDisplayImmediateItems](./getdisplayimmediateitems/) | Gibt an, ob Elemente im Zeilen- und Spaltenbereich sichtbar sind, wenn der Datenbereich der PivotTable leer ist. Der Standardwert ist true. |
| [SetDisplayImmediateItems](./setdisplayimmediateitems/) | Gibt an, ob Elemente im Zeilen- und Spaltenbereich sichtbar sind, wenn der Datenbereich der PivotTable leer ist. Der Standardwert ist true. |
| [IsSelected](./isselected/) | Gibt an, ob diese PivotTable ausgewählt ist. |
| [SetIsSelected](./setisselected/) | Gibt an, ob diese PivotTable ausgewählt ist. |
| [GetShowPivotStyleRowHeader](./getshowpivotstylerowheader/) | Gibt an, ob die Zeilenüberschrift in der PivotTable den Stil erhalten soll. |
| [SetShowPivotStyleRowHeader](./setshowpivotstylerowheader/) | Gibt an, ob die Zeilenüberschrift in der PivotTable den Stil erhalten soll. |
| [GetShowPivotStyleColumnHeader](./getshowpivotstylecolumnheader/) | Gibt an, ob die Spaltenüberschrift in der PivotTable den Stil erhalten soll. |
| [SetShowPivotStyleColumnHeader](./setshowpivotstylecolumnheader/) | Gibt an, ob die Spaltenüberschrift in der PivotTable den Stil erhalten soll. |
| [GetShowPivotStyleRowStripes](./getshowpivotstylerowstripes/) | Gibt an, ob Zeilenstreifenformatierung angewendet wird. |
| [SetShowPivotStyleRowStripes](./setshowpivotstylerowstripes/) | Gibt an, ob Zeilenstreifenformatierung angewendet wird. |
| [GetShowPivotStyleColumnStripes](./getshowpivotstylecolumnstripes/) | Gibt an, ob Streifenformatierung für Spalten angewendet wird. |
| [SetShowPivotStyleColumnStripes](./setshowpivotstylecolumnstripes/) | Gibt an, ob Streifenformatierung für Spalten angewendet wird. |
| [GetShowPivotStyleLastColumn](./getshowpivotstylelastcolumn/) | Gibt an, ob die Spaltenformatierung angewendet wird. |
| [SetShowPivotStyleLastColumn](./setshowpivotstylelastcolumn/) | Gibt an, ob die Spaltenformatierung angewendet wird. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Ermittelt die horizontalen Seitenumbrüche dieser PivotTable. |
| [ShowInCompactForm](./showincompactform/) | Gestaltet die PivotTable-Ansicht in kompakter Form. |
| [ShowInOutlineForm](./showinoutlineform/) | Gestaltet die PivotTable in Gliederungsform. |
| [ShowInTabularForm](./showintabularform/) | Gestaltet die PivotTable in Tabellenform. |
| [GetCellByDisplayName](./getcellbydisplayname/) | Ermittelt das Zellobjekt anhand des Anzeigenamens des PivotField. |
| [GetDependentPivotTables](./getdependentpivottables/) | Ermittelt alle PivotTables, die diese PivotTable als Datenquelle verwenden. |
| [ExportViewToJson](./exportviewtojson/) | Exportiert die Pivot-Ansicht als JSON. |
