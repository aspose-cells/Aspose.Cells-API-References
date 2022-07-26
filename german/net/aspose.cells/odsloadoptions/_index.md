---
title: OdsLoadOptions
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert die Optionen zum Laden der ODS-Datei.
type: docs
weight: 4330
url: /de/net/aspose.cells/odsloadoptions/
---
## OdsLoadOptions class

Repräsentiert die Optionen zum Laden der ODS-Datei.

```csharp
public class OdsLoadOptions : LoadOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [OdsLoadOptions](odsloadoptions#constructor)() | Repräsentiert die Optionen zum Laden der ODS-Datei. |
| [OdsLoadOptions](odsloadoptions#constructor_1)(LoadFormat) | Repräsentiert die Optionen zum Laden der ODS-Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ApplyExcelDefaultStyleToHyperlink](../../aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink) { get; set; } | Gibt an, ob der Standardstil von Excel auf den Hyperlink angewendet wird. |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Ruft die Autofitter-Optionen ab und legt sie fest |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Prüfen, ob Daten in der Vorlagendatei gültig sind. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Ob die Einschränkung der Excel-Datei überprüft wird, wenn der Benutzer zellenbezogene Objekte ändert. Zum Beispiel erlaubt Excel keine Eingabe von Zeichenfolgenwerten, die länger als 32 KB sind. Wenn Sie einen Wert eingeben, der länger als 32 KB ist, wie z Eigenschaft wahr ist, erhalten Sie eine Ausnahme. Wenn diese Eigenschaft falsch ist, akzeptieren wir Ihren eingegebenen Zeichenfolgenwert als Wert der Zelle, sodass Sie später den vollständigen Zeichenfolgenwert für andere Dateiformate wie CSV ausgeben können. Wenn jedoch Sie haben einen Wert festgelegt, der für das Excel-Dateiformat ungültig ist. Sie sollten die Arbeitsmappe später nicht im Excel-Dateiformat speichern. Andernfalls kann es zu einem unerwarteten Fehler für die generierte Excel-Datei kommen. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Ruft die Systemkulturinformationen zum Zeitpunkt des Ladens der Datei ab oder legt sie fest. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Ruft die Standardstileinstellungen zum Initialisieren von Stilen der Arbeitsmappe ab |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Holt und setzt individuelle Schriftkonfigurationen. Funktioniert nur für die[`Workbook`](../workbook) der das nutzt[`LoadOptions`](../loadoptions) zu laden.&gt; |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Ignorieren Sie die Daten, die nicht gedruckt werden, wenn Sie die Datei direkt drucken |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Holt und setzt den Interrupt-Monitor. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Ob die ungeparsten Daten für die Arbeitsmappe im Speicher bleiben, wenn sie aus der Vorlagendatei geladen wird. Standard ist wahr. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Ruft die Sprache der Benutzeroberfläche der Workbook-Version ab oder legt sie fest, basierend auf dem CountryCode, der die Datei gespeichert hat. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Der Datenhandler zum Verarbeiten von Zellendaten beim Lesen der Vorlagendatei. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Der Filter, um anzugeben, wie Daten geladen werden. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Ruft das Ladeformat ab. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Ruft die Speichernutzungsoptionen ab oder legt sie fest. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Gibt an, ob die Formel beim Lesen der Datei analysiert wird. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Gibt an, ob beim Laden der Datei zwischengespeicherte Pivot-Datensätze analysiert werden. Der Standardwert ist „false“. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Ruft das Passwort der Arbeitsmappe ab und legt es fest. |
| [RefreshPivotTables](../../aspose.cells/odsloadoptions/refreshpivottables) { get; set; } | Gibt an, ob Pivot-Tabellen beim Laden der Datei aktualisiert werden. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Ruft die Ländereinstellungen des Systems basierend auf CountryCode zum Zeitpunkt des Ladens der Datei ab oder legt diese fest. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Ruft Warnrückruf ab oder legt ihn fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Legt das Standarddruckpapierformat aus der Standarddruckereinstellung fest. |

### Siehe auch

* class [LoadOptions](../loadoptions)
* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
