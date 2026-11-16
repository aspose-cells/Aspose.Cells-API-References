---
title: "Workbook Klasse"
linktitle: "Workbook"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "Workbook Klasse. Kapselt das Objekt, das das Workbook in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/workbook/
---

## Workbook class

Stellt ein Root‑Objekt zum Erstellen einer Excel‑Tabelle dar.

```go

type Workbook struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewWorkbook](./newworkbook/) | Initialisiert eine neue Instanz der Workbook-Klasse. |
| [NewWorkbook_FileFormatType](./newworkbook_fileformattype/) | Initialisiert eine neue Instanz der Workbook-Klasse. |
| [NewWorkbook_LoadOptions](./newworkbook_loadoptions/) | Initialisiert eine neue leere Instanz der Workbook-Klasse mit Optionen |
| [NewWorkbook_String](./newworkbook_string/) | Initialisiert eine neue Instanz der Workbook-Klasse und öffnet eine Datei. |
| [NewWorkbook_Stream](./newworkbook_stream/) | Initialisiert eine neue Instanz der Workbook-Klasse und öffnet einen Stream. |
| [NewWorkbook_String_LoadOptions](./newworkbook_string_loadoptions/) | Initialisiert eine neue Instanz der Workbook-Klasse und öffnet eine Datei. |
| [NewWorkbook_Stream_LoadOptions](./newworkbook_stream_loadoptions/) | Initialisiert eine neue Instanz der Workbook-Klasse und öffnet den Stream. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetSettings](./getsettings/) | Stellt die Workbook-Einstellungen dar. |
| [ParseFormulas](./parseformulas/) | Parst alle Formeln, die nicht geparst wurden, als sie aus einer Vorlagendatei geladen oder einer Zelle zugewiesen wurden. |
| [StartAccessCache](./startaccesscache/) | Startet die Sitzung, die Caches verwendet, um auf Daten zuzugreifen. |
| [CloseAccessCache](./closeaccesscache/) | Schließt die Sitzung, die Caches verwendet, um auf Daten zuzugreifen. |
| [Save_String_SaveFormat](./save_string_saveformat/) | Speichert das Workbook auf der Festplatte. |
| [Save_String](./save_string/) | Speichere das Workbook auf der Festplatte. |
| [Save_String_SaveOptions](./save_string_saveoptions/) | Speichert das Workbook auf der Festplatte. |
| [Save_SaveFormat](./save_saveformat/) | Speichert das Workbook in den Stream. |
| [Save_SaveOptions](./save_saveoptions/) | Speichert das Workbook in den Stream. |
| [SaveToStream](./savetostream/) | Speichert die Excel-Datei in ein MemoryStream-Objekt als Excel97-2003 xls-Datei und gibt es zurück. |
| [GetWorksheets](./getworksheets/) | Ruft die WorksheetCollection-Sammlung in der Tabellenkalkulation ab. |
| [IsLicensed](./islicensed/) | Gibt an, ob die Lizenz gesetzt ist. |
| [RemoveUnusedStyles](./removeunusedstyles/) | Entfernt alle ungenutzten Stile. |
| [CreateStyle](./createstyle/) | Erstellt einen neuen Stil. |
| [CreateStyle_Bool](./createstyle_bool/) | Erstellt einen neuen Stil. |
| [CreateBuiltinStyle](./createbuiltinstyle/) | Erstellt einen integrierten Stil anhand des angegebenen Typs. |
| [CreateCellsColor](./createcellscolor/) | Erstellt ein CellsColor-Objekt. |
| [Replace_String_String](./replace_string_string/) | Ersetzt den Wert einer Zelle durch einen neuen String. |
| [Replace_String_Int](./replace_string_int/) | Ersetzt den Wert einer Zelle durch eine neue Ganzzahl. |
| [Replace_String_Double](./replace_string_double/) | Ersetzt den Wert einer Zelle durch einen neuen Double-Wert. |
| [Replace_String_stringArray_Bool](./replace_string_stringarray_bool/) | Ersetzt den Wert einer Zelle durch ein neues String-Array. |
| [Replace_String_int32Array_Bool](./replace_string_int32array_bool/) | Ersetzt die Werte mehrerer Zellen durch ein Integer-Array. |
| [Replace_String_float64Array_Bool](./replace_string_float64array_bool/) | Ersetzt die Werte mehrerer Zellen durch ein Double-Array. |
| [Replace_Bool_Object](./replace_bool_object/) | Ersetzt die Werte mehrerer Zellen durch neue Daten. |
| [Replace_Int_Object](./replace_int_object/) | Ersetzt die Werte mehrerer Zellen durch neue Daten. |
| [Replace_String_String_ReplaceOptions](./replace_string_string_replaceoptions/) | Ersetzt den Wert einer Zelle durch einen neuen String. |
| [Copy_Workbook_CopyOptions](./copy_workbook_copyoptions/) | Kopiert ein weiteres Workbook-Objekt. |
| [Copy_Workbook](./copy_workbook/) | Kopiert Daten aus einem Quell-Workbook-Objekt. |
| [Combine](./combine/) | Kombiniert ein weiteres Workbook-Objekt. |
| [GetColors](./getcolors/) | Gibt die Farben in der Palette für das Tabellenblatt zurück. |
| [GetStyleInPool](./getstyleinpool/) | Liest den Stil im Stil-Pool. Alle Stile im Workbook werden in einen Pool gesammelt. In den Zellen gibt es nur einen einfachen Referenzindex. |
| [GetCountOfStylesInPool](./getcountofstylesinpool/) | Liest die Anzahl der Stile im Stil-Pool. |
| [GetFonts](./getfonts/) | Liest alle Schriftarten im Stil-Pool. |
| [GetNamedStyle](./getnamedstyle/) | Liest den benannten Stil im Stil-Pool. |
| [MergeNamedStyles](./mergenamedstyles/) | Führt benannte Stile aus der anderen Excel-Datei zusammen. |
| [ChangePalette](./changepalette/) | Ändert die Palette für das Tabellenblatt am angegebenen Index. |
| [IsColorInPalette](./iscolorinpalette/) | Prüft, ob eine Farbe in der Palette für das Tabellenblatt enthalten ist. |
| [CalculateFormula](./calculateformula/) | Berechnet das Ergebnis von Formeln. |
| [CalculateFormula_Bool](./calculateformula_bool/) | Berechnet das Ergebnis von Formeln. |
| [CalculateFormula_CalculationOptions](./calculateformula_calculationoptions/) | Berechnet Formeln in diesem Workbook. |
| [RefreshDynamicArrayFormulas_Bool](./refreshdynamicarrayformulas_bool/) | Aktualisiert dynamische Array-Formeln (erweitert sich in einen neuen Bereich benachbarter Zellen gemäß den aktuellen Daten). Andere Formeln im Workbook werden nicht rekursiv berechnet, selbst wenn sie von dynamischen Array-Formeln verwendet wurden. |
| [RefreshDynamicArrayFormulas_Bool_CalculationOptions](./refreshdynamicarrayformulas_bool_calculationoptions/) | Aktualisiert dynamische Array-Formeln (erweitert sich in einen neuen Bereich benachbarter Zellen gemäß den aktuellen Daten) |
| [GetDefaultStyle](./getdefaultstyle/) | Liest oder setzt das Standard‑Style‑Objekt des Workbooks. |
| [SetDefaultStyle](./setdefaultstyle/) | Liest oder setzt das Standard‑Style‑Objekt des Workbooks. |
| [GetMatchingColor](./getmatchingcolor/) | Finde die am besten passende Farbe in der aktuellen Palette. |
| [IsDigitallySigned](./isdigitallysigned/) | Zeigt an, ob diese Tabelle digital signiert ist. |
| [SetEncryptionOptions](./setencryptionoptions/) | Verschlüsselungsoptionen festlegen. |
| [Protect](./protect/) | Schützt eine Arbeitsmappe. |
| [ProtectSharedWorkbook](./protectsharedworkbook/) | Schützt eine freigegebene Arbeitsmappe. |
| [Unprotect](./unprotect/) | Hebt den Schutz einer Arbeitsmappe auf. |
| [UnprotectSharedWorkbook](./unprotectsharedworkbook/) | Hebt den Schutz einer freigegebenen Arbeitsmappe auf. |
| [IsWorkbookProtectedWithPassword](./isworkbookprotectedwithpassword/) | Zeigt an, ob Struktur oder Fenster mit einem Passwort geschützt ist. |
| [RemoveMacro](./removemacro/) | Entfernt VBA/Makro aus dieser Tabelle. |
| [GetVbaProject](./getvbaproject/) | Ruft das VbaProject in einer Tabelle ab. |
| [RemoveDigitalSignature](./removedigitalsignature/) | Entfernt die digitale Signatur aus dieser Tabelle. |
| [AcceptAllRevisions](./acceptallrevisions/) | Akzeptiert alle nachverfolgten Änderungen in der Arbeitsmappe. |
| [GetHasMacro](./gethasmacro/) | Zeigt an, ob diese Tabelle Makro/VBA enthält. |
| [GetHasRevisions](./gethasrevisions/) | Ermittelt, ob die Arbeitsmappe nachverfolgte Änderungen hat |
| [GetFileName](./getfilename/) | Liest und legt den aktuellen Dateinamen fest. |
| [SetFileName](./setfilename/) | Liest und legt den aktuellen Dateinamen fest. |
| [GetDataSorter](./getdatasorter/) | Ruft ein DataSorter-Objekt zum Sortieren von Daten ab. |
| [GetThemeColor](./getthemecolor/) | Liest die Designfarbe. |
| [SetThemeColor](./setthemecolor/) | Legt die Designfarbe fest |
| [GetTheme](./gettheme/) | Liest den Designnamen. |
| [CustomTheme](./customtheme/) | Passt das Design an. |
| [CopyTheme](./copytheme/) | Kopiert das Design aus einer anderen Arbeitsmappe. |
| [UpdateCustomFunctionDefinition](./updatecustomfunctiondefinition/) | Aktualisiert die Definition benutzerdefinierter Funktionen. |
| [UpdateLinkedDataSource](./updatelinkeddatasource/) | Wenn diese Arbeitsmappe externe Verknüpfungen zu anderen Datenquellen enthält, wird Aspose.Cells versuchen, die neuesten Daten aus den angegebenen Quellen abzurufen. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Gibt eine DocumentProperty‑Sammlung zurück, die alle integrierten Dokumenteigenschaften der Tabelle darstellt. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Gibt eine DocumentProperty‑Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Tabelle darstellt. |
| [GetFileFormat](./getfileformat/) | Liest und setzt das Dateiformat. |
| [SetFileFormat](./setfileformat/) | Liest und setzt das Dateiformat. |
| [GetHasCustomFunction](./gethascustomfunction/) | Ermittelt, ob im Arbeitsbuch benutzerdefinierte Funktionen verwendet werden, z. B. in Zellformeln oder definierten Namen... |
| [GetInterruptMonitor](./getinterruptmonitor/) | Liest und setzt den Interrupt‑Monitor. |
| [SetInterruptMonitor_AbstractInterruptMonitor](./setinterruptmonitor_abstractinterruptmonitor/) | Liest und setzt den Interrupt‑Monitor. |
| [SetInterruptMonitor_InterruptMonitor](./setinterruptmonitor_interruptmonitor/) | Setzt den Interrupt‑Monitor. |
| [GetContentTypeProperties](./getcontenttypeproperties/) | Liest die Liste der ContentTypeProperty‑Objekte im Arbeitsbuch. |
| [GetCustomXmlParts](./getcustomxmlparts/) | Stellt einen benutzerdefinierten XML-Datenspeicherteil dar (benutzerdefinierte XML-Daten innerhalb eines Pakets). |
| [GetDataMashup](./getdatamashup/) | Liest Mashup‑Daten. |
| [GetRibbonXml](./getribbonxml/) | Liest und setzt die XML‑Datei, die die Ribbon‑UI definiert. |
| [SetRibbonXml](./setribbonxml/) | Liest und setzt die XML‑Datei, die die Ribbon‑UI definiert. |
| [GetAbsolutePath](./getabsolutepath/) | Liest und setzt den absoluten Pfad der Datei. |
| [SetAbsolutePath](./setabsolutepath/) | Liest und setzt den absoluten Pfad der Datei. |
| [GetDataConnections](./getdataconnections/) | Liest die ExternalConnection‑Sammlung. |
| [ImportXml_String_String_Int_Int](./importxml_string_string_int_int/) | Importiert/Aktualisiert eine XML‑Datendatei im Arbeitsbuch. |
| [ImportXml_Stream_String_Int_Int](./importxml_stream_string_int_int/) | Importiert/Aktualisiert eine XML‑Datendatei im Arbeitsbuch. |
| [ExportXml_String_String](./exportxml_string_string/) | Exportiert XML‑Daten, die durch die angegebene XML‑Zuordnung verknüpft sind. |
| [ExportXml_String](./exportxml_string/) | Exportiert XML‑Daten. |
| [SetDigitalSignature](./setdigitalsignature/) | Setzt eine digitale Signatur für eine Tabellenkalkulationsdatei (Excel2007 und neuer). |
| [AddDigitalSignature](./adddigitalsignature/) | Fügt einer OOXML‑Tabellenkalkulationsdatei (Excel2007 und neuer) eine digitale Signatur hinzu. |
| [GetDigitalSignature](./getdigitalsignature/) | Liest die digitale Signatur aus der Datei. |
| [RemovePersonalInformation](./removepersonalinformation/) | Entfernt persönliche Informationen. |
| [GetDataModel](./getdatamodel/) | Liest das Datenmodell im Arbeitsbuch. |
| [RefreshAll](./refreshall/) | Aktualisiert verknüpfte Formen, alle Pivot‑Tabellen und Diagramme mit Pivot‑Quelle. |
| [Dispose](./dispose/) | Führt anwendungsspezifische Aufgaben aus, die mit dem Freigeben, Freisetzen oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
