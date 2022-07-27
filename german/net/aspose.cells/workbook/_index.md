---
title: Workbook
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert ein Stammobjekt zum Erstellen einer Excel-Tabelle.
type: docs
weight: 6480
url: /de/net/aspose.cells/workbook/
---
## Workbook class

Repräsentiert ein Stammobjekt zum Erstellen einer Excel-Tabelle.

```csharp
public class Workbook : IDisposable
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [Workbook](workbook#constructor)() | Initialisiert eine neue Instanz von[`Workbook`](../workbook) Klasse. |
| [Workbook](workbook#constructor_1)(FileFormatType) | Initialisiert eine neue Instanz von[`Workbook`](../workbook) Klasse. |
| [Workbook](workbook#constructor_2)(Stream) | Initialisiert eine neue Instanz von[`Workbook`](../workbook) Klasse und öffne einen Stream. |
| [Workbook](workbook#constructor_4)(string) | Initialisiert eine neue Instanz von[`Workbook`](../workbook) Klasse und öffnen Sie eine Datei. |
| [Workbook](workbook#constructor_3)(Stream, LoadOptions) | Initialisiert eine neue Instanz von[`Workbook`](../workbook) Klasse und offener Stream. |
| [Workbook](workbook#constructor_5)(string, LoadOptions) | Initialisiert eine neue Instanz von[`Workbook`](../workbook) Klasse und öffnen Sie eine Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath) { get; set; } | Holt und setzt den absoluten Pfad der Datei. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties) { get; } | Gibt a zurück[`DocumentProperty`](../../aspose.cells.properties/documentproperty)Sammlung, die alle integrierten Dokumenteigenschaften der Tabelle darstellt. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory) { get; } | Ruft die Factory zum Erstellen von ICellsDataTable aus benutzerdefinierten Objekten ab |
| [Colors](../../aspose.cells/workbook/colors) { get; } | Gibt Farben in der Palette für die Tabelle zurück. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties) { get; } | Ruft die Liste von ab[`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty) Objekte in der Arbeitsmappe. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool) { get; } | Ruft die Anzahl der Styles im Style-Pool ab. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties) { get; } | Gibt a zurück[`DocumentProperty`](../../aspose.cells.properties/documentproperty) Sammlung, die alle benutzerdefinierten Dokumenteigenschaften der Tabelle darstellt. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts) { get; } | Repräsentiert einen benutzerdefinierten XML-Datenspeicherteil (benutzerdefinierte XML-Daten innerhalb eines Pakets). |
| [DataConnections](../../aspose.cells/workbook/dataconnections) { get; } | Ruft die ab[`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection) Sammlung. |
| [DataMashup](../../aspose.cells/workbook/datamashup) { get; } | Ruft Mashup-Daten ab. |
| [DataSorter](../../aspose.cells/workbook/datasorter) { get; } | Ruft ein DataSorter-Objekt ab, um Daten zu sortieren. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle) { get; set; } | Ruft den Standardwert ab oder legt ihn fest[`Style`](../style) Objekt der Arbeitsmappe. |
| [FileFormat](../../aspose.cells/workbook/fileformat) { get; set; } | Ruft das Dateiformat ab und legt es fest. |
| [FileName](../../aspose.cells/workbook/filename) { get; set; } | Holt und setzt den aktuellen Dateinamen. |
| [HasMacro](../../aspose.cells/workbook/hasmacro) { get; } | Gibt an, ob diese Tabelle Makros/VBA enthält. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions) { get; } | Ruft ab, ob die Arbeitsmappe nachverfolgte Änderungen aufweist |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor) { get; set; } | Holt und setzt den Interrupt-Monitor. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned) { get; } | Gibt an, ob diese Tabelle digital signiert ist. |
| [IsLicensed](../../aspose.cells/workbook/islicensed) { get; } | Zeigt an, ob die Lizenz gesetzt ist. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword) { get; } | Zeigt an, ob die Struktur oder das Fenster mit einem Passwort geschützt ist. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml) { get; set; } | Ruft die XML-Datei ab und legt sie fest, die die Multifunktionsleisten-Benutzeroberfläche definiert. |
| [Settings](../../aspose.cells/workbook/settings) { get; } | Stellt die Arbeitsmappeneinstellungen dar. |
| [Theme](../../aspose.cells/workbook/theme) { get; } | Ruft den Themennamen ab. |
| [VbaProject](../../aspose.cells/workbook/vbaproject) { get; } | Ruft die ab[`VbaProject`](./vbaproject) in einer Tabelle. |
| [Worksheets](../../aspose.cells/workbook/worksheets) { get; } | Ruft die ab[`WorksheetCollection`](../worksheetcollection) Sammlung in der Tabelle. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions)() | Akzeptiert alle nachverfolgten Änderungen in der Arbeitsmappe. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature)(DigitalSignatureCollection) | Fügt einer OOXML-Tabellenkalkulationsdatei (Excel2007 und höher) eine digitale Signatur hinzu. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula)() | Berechnet das Ergebnis von Formeln. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_2)(bool) | Berechnet das Ergebnis von Formeln. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_1)(CalculationOptions) | Formeln in dieser Arbeitsmappe berechnen. |
| [ChangePalette](../../aspose.cells/workbook/changepalette)(Color, int) | Ändert die Palette für die Tabelle im angegebenen Index. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache)(AccessCacheOptions) | Schließt die Sitzung, die Caches verwendet, um auf Daten zuzugreifen. |
| [Combine](../../aspose.cells/workbook/combine)(Workbook) | Kombiniert ein anderes Workbook-Objekt. |
| [Copy](../../aspose.cells/workbook/copy#copy)(Workbook) | Kopiert Daten aus einem Arbeitsmappen-Quellobjekt. |
| [Copy](../../aspose.cells/workbook/copy#copy_1)(Workbook, CopyOptions) | Kopiert Daten aus einem Arbeitsmappen-Quellobjekt. |
| [CopyTheme](../../aspose.cells/workbook/copytheme)(Workbook) | Kopiert das Design aus einer anderen Arbeitsmappe. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle)(BuiltinStyleType) | Erstellt einen integrierten Stil nach gegebenem Typ. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor)() | Erstellt ein[`CellsColor`](../cellscolor) Objekt. |
| [CreateStyle](../../aspose.cells/workbook/createstyle)() | Erstellt einen neuen Stil. |
| [CustomTheme](../../aspose.cells/workbook/customtheme)(string, Color[]) | Passt das Thema an. |
| [Dispose](../../aspose.cells/workbook/dispose)() | Führt anwendungsdefinierte Aufgaben aus, die mit dem Freigeben, Freigeben oder Zurücksetzen nicht verwalteter Ressourcen verbunden sind. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml)(string, Stream) | XML-Daten exportieren. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml_1)(string, string) | XML-Daten exportieren, die durch die angegebene XML-Zuordnung verknüpft sind. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature)() | Ruft digitale Signatur aus Datei ab. |
| [GetFonts](../../aspose.cells/workbook/getfonts)() | Ruft alle Schriftarten im Style-Pool ab. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor)(Color) | Finden Sie die am besten passende Farbe in der aktuellen Palette. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle)(string) | Ruft den benannten Stil im Stilpool ab. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool)(int) | Holt den Stil in den Stilpool. Alle Stile in der Arbeitsmappe werden in einem Pool gesammelt. Es gibt nur einen einfachen Referenzindex in den Zellen. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor)(ThemeColorType) | Ruft Designfarbe ab. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml)(Stream, string, int, int) | Importiert/aktualisiert eine XML-Datendatei in die Arbeitsmappe. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml_1)(string, string, int, int) | Importiert/aktualisiert eine XML-Datendatei in die Arbeitsmappe. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette)(Color) | Überprüft, ob eine Farbe in der Palette für die Tabelle enthalten ist. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas)(bool) | Analysiert alle Formeln, die nicht analysiert wurden, als sie aus der Vorlagendatei geladen oder in eine Zelle gesetzt wurden. |
| [Protect](../../aspose.cells/workbook/protect)(ProtectionType, string) | Schützt eine Arbeitsmappe. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook)(string) | Schützt eine freigegebene Arbeitsmappe. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas)(bool) | Aktualisiert dynamische Array-Formeln (Überlauf in einen neuen Bereich benachbarter Zellen gemäß den aktuellen Daten) |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature)() | Entfernt die digitale Signatur aus dieser Tabelle. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro)() | Entfernt VBA/Makro aus dieser Tabelle. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation)() | Entfernt persönliche Informationen. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles)() | Entfernen Sie alle nicht verwendeten Stile. |
| [Replace](../../aspose.cells/workbook/replace#replace)(bool, object) | Ersetzt die Werte der Zellen durch neue Daten. |
| [Replace](../../aspose.cells/workbook/replace#replace_1)(int, object) | Ersetzt die Werte der Zellen durch neue Daten. |
| [Replace](../../aspose.cells/workbook/replace#replace_6)(string, DataTable) | Ersetzt die Werte der Zellen durch Daten aus aDataTable . |
| [Replace](../../aspose.cells/workbook/replace#replace_2)(string, double) | Ersetzt den Wert einer Zelle durch ein neues Double. |
| [Replace](../../aspose.cells/workbook/replace#replace_4)(string, int) | Ersetzt den Wert einer Zelle durch eine neue Ganzzahl. |
| [Replace](../../aspose.cells/workbook/replace#replace_7)(string, string) | Ersetzt den Wert einer Zelle durch eine neue Zeichenfolge. |
| [Replace](../../aspose.cells/workbook/replace#replace_3)(string, double[], bool) | Ersetzt die Werte der Zellen durch ein doppeltes Array. |
| [Replace](../../aspose.cells/workbook/replace#replace_5)(string, int[], bool) | Ersetzt die Werte der Zellen durch ein Integer-Array. |
| [Replace](../../aspose.cells/workbook/replace#replace_8)(string, string, ReplaceOptions) | Ersetzt den Wert einer Zelle durch eine neue Zeichenfolge. |
| [Replace](../../aspose.cells/workbook/replace#replace_9)(string, string[], bool) | Ersetzt den Wert einer Zelle durch ein neues String-Array. |
| [Save](../../aspose.cells/workbook/save#save_2)(string) | Speichern Sie die Arbeitsmappe auf der Festplatte. |
| [Save](../../aspose.cells/workbook/save#save)(Stream, SaveFormat) | Speichert die Arbeitsmappe im Stream. |
| [Save](../../aspose.cells/workbook/save#save_1)(Stream, SaveOptions) | Speichert die Arbeitsmappe im Stream. |
| [Save](../../aspose.cells/workbook/save#save_3)(string, SaveFormat) | Speichert die Arbeitsmappe auf der Festplatte. |
| [Save](../../aspose.cells/workbook/save#save_4)(string, SaveOptions) | Speichert die Arbeitsmappe auf der Festplatte. |
| [Save](../../aspose.cells/workbook/save#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Erstellt die Ergebnistabelle und überträgt sie an den Client, öffnet sie dann im Browser oder in MS Workbook. |
| [Save](../../aspose.cells/workbook/save#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Erstellt die Ergebnistabelle und überträgt sie an den Client, öffnet sie dann im Browser oder in MS Workbook. |
| [SaveToStream](../../aspose.cells/workbook/savetostream)() | Speichert eine Excel-Datei in einem MemoryStream-Objekt und gibt sie zurück. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature)(DigitalSignatureCollection) | Setzt eine digitale Signatur auf eine Tabellenkalkulationsdatei (Excel2007 und höher). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions)(EncryptionType, int) | Verschlüsselungsoptionen festlegen. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor)(ThemeColorType, Color) | Legt die Designfarbe fest |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache)(AccessCacheOptions) | Startet die Sitzung, die Caches verwendet, um auf Daten zuzugreifen. |
| [Unprotect](../../aspose.cells/workbook/unprotect)(string) | Hebt den Schutz einer Arbeitsmappe auf. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook)(string) | Hebt den Schutz einer freigegebenen Arbeitsmappe auf. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource)(Workbook[]) | Wenn diese Arbeitsmappe externe Links zu anderen Datenquellen enthält, wird Aspose.Cells versuchen, die neuesten Daten abzurufen. |

### Bemerkungen

Die Workbook-Klasse bezeichnet eine Excel-Tabelle. Jede Tabelle kann mehrere Arbeitsblätter enthalten. Die grundlegende Funktion der Klasse besteht darin, native Excel-Dateien zu öffnen und zu speichern. Die Klasse verfügt über einige erweiterte Funktionen wie das Kopieren von Daten aus anderen Arbeitsmappen, das Kombinieren von zwei Arbeitsmappen und das Schützen der Excel-Tabelle.

### Beispiele

Das folgende Beispiel lädt eine Arbeitsmappe aus einer Datei namens designer.xls und macht die horizontalen und vertikalen Bildlaufleisten für die Arbeitsmappe unsichtbar. Es ersetzt dann zwei String-Werte durch einen Integer-Wert bzw. einen String-Wert innerhalb der Tabelle und sendet schließlich die aktualisierte Datei an den Client-Browser.

```csharp
[C#]

//Öffne eine Designer-Datei
string designerFile = "designer.xls";
Workbook workbook = new Workbook(designerFile);

//Bildlaufleisten setzen
workbook.Settings.IsHScrollBarVisible = false;
workbook.Settings.IsVScrollBarVisible = false;

//Ersetzen Sie die Platzhalterzeichenfolge durch neue Werte
int newInt = 100;
workbook.Replace("OldInt", newInt);

string newString = "Hello!";
workbook.Replace("OldString", newString);
workbook.Save("result.xls");

[Visual Basic]

'Öffnen Sie eine Designerdatei
Dim designerFile as String = "\designer.xls"
Dim workbook as Workbook = new Workbook(designerFile)

'Bildlaufleisten einstellen
workbook.IsHScrollBarVisible = False
workbook.IsVScrollBarVisible = False

'Ersetzen Sie die Platzhalterzeichenfolge durch neue Werte
Dim newInt as Integer = 100
workbook.Replace("OldInt", newInt)

Dim newString as String = "Hello!"
workbook.Replace("OldString", newString)
workbook.Save("result.xls")    
```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
