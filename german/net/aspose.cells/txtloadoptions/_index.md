---
title: TxtLoadOptions
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert die Optionen zum Laden einer Textdatei.
type: docs
weight: 6110
url: /de/net/aspose.cells/txtloadoptions/
---
## TxtLoadOptions class

Repräsentiert die Optionen zum Laden einer Textdatei.

```csharp
public class TxtLoadOptions : AbstractTextLoadOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [TxtLoadOptions](txtloadoptions#constructor)() | Erstellt die Optionen zum Laden einer Textdatei. |
| [TxtLoadOptions](txtloadoptions#constructor_1)(LoadFormat) | Erstellt die Optionen zum Laden einer Textdatei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Ruft die Autofitter-Optionen ab und legt sie fest |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Prüfen, ob Daten in der Vorlagendatei gültig sind. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Ob die Einschränkung der Excel-Datei überprüft wird, wenn der Benutzer zellenbezogene Objekte ändert. Zum Beispiel erlaubt Excel keine Eingabe von Zeichenfolgenwerten, die länger als 32 KB sind. Wenn Sie einen Wert eingeben, der länger als 32 KB ist, wie z Eigenschaft wahr ist, erhalten Sie eine Ausnahme. Wenn diese Eigenschaft falsch ist, akzeptieren wir Ihren eingegebenen Zeichenfolgenwert als Wert der Zelle, sodass Sie später den vollständigen Zeichenfolgenwert für andere Dateiformate wie CSV ausgeben können. Wenn jedoch Sie haben einen Wert festgelegt, der für das Excel-Dateiformat ungültig ist. Sie sollten die Arbeitsmappe später nicht im Excel-Dateiformat speichern. Andernfalls kann es zu einem unerwarteten Fehler für die generierte Excel-Datei kommen. |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die Zeichenfolge in der Textdatei in Datumsdaten konvertiert wird. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die Zeichenfolge in der Textdatei in numerische Daten konvertiert wird. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Ruft die Systemkulturinformationen zum Zeitpunkt des Ladens der Datei ab oder legt sie fest. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Ruft die Standardstileinstellungen zum Initialisieren von Stilen der Arbeitsmappe ab |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding) { get; set; } | Ruft die Standardcodierung ab und legt sie fest. Gilt nur für csv-Datei. |
| [ExtendToNextSheet](../../aspose.cells/txtloadoptions/extendtonextsheet) { get; set; } | Ob Daten auf das nächste Blatt erweitert werden, wenn die Zeilen oder Spalten der Daten das Limit überschreiten. Wenn diese Eigenschaft wahr ist, werden zusätzliche Daten auf das nächste Blatt hinter dem aktuellen erweitert (wenn das aktuelle Blatt das letzte ist, wird ein neues Blatt angehängt zur aktuellen Arbeitsmappe). Wenn diese Eigenschaft falsch ist, wird die Datenüberschreitung ignoriert. Standard ist falsch; |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Holt und setzt individuelle Schriftkonfigurationen. Funktioniert nur für die[`Workbook`](../workbook) der das nutzt[`LoadOptions`](../loadoptions) zu laden.&gt; |
| [HasFormula](../../aspose.cells/txtloadoptions/hasformula) { get; set; } | Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt. |
| [HasTextQualifier](../../aspose.cells/txtloadoptions/hastextqualifier) { get; set; } | Ob es einen Textbezeichner für den Zellenwert gibt. Standard ist wahr. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Ignorieren Sie die Daten, die nicht gedruckt werden, wenn Sie die Datei direkt drucken |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Holt und setzt den Interrupt-Monitor. |
| [IsMultiEncoded](../../aspose.cells/txtloadoptions/ismultiencoded) { get; set; } | True bedeutet, dass die Datei mehrere Kodierungen enthält. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision) { get; set; } | Gibt an, ob ein Zeichenfolgenwert nicht analysiert wird, wenn die Länge 15 beträgt. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Ob die ungeparsten Daten für die Arbeitsmappe im Speicher bleiben, wenn sie aus der Vorlagendatei geladen wird. Standard ist wahr. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Ruft die Sprache der Benutzeroberfläche der Workbook-Version ab oder legt sie fest, basierend auf dem CountryCode, der die Datei gespeichert hat. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Der Datenhandler zum Verarbeiten von Zellendaten beim Lesen der Vorlagendatei. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Der Filter, um anzugeben, wie Daten geladen werden. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Ruft das Ladeformat ab. |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy) { get; set; } | Gibt die Strategie zum Anwenden des Stils für geparste Werte an, wenn der Zeichenfolgenwert in eine Zahl oder Datumszeit konvertiert wird. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Ruft die Speichernutzungsoptionen ab oder legt sie fest. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Gibt an, ob die Formel beim Lesen der Datei analysiert wird. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Gibt an, ob beim Laden der Datei zwischengespeicherte Pivot-Datensätze analysiert werden. Der Standardwert ist „false“. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Ruft das Passwort der Arbeitsmappe ab und legt es fest. |
| [PreferredParsers](../../aspose.cells/txtloadoptions/preferredparsers) { get; set; } | Ruft bevorzugte Wertparser zum Laden von Textdateien ab und legt sie fest. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Ruft die Ländereinstellungen des Systems basierend auf CountryCode zum Zeitpunkt des Ladens der Datei ab oder legt diese fest. |
| [Separator](../../aspose.cells/txtloadoptions/separator) { get; set; } | Liest und setzt Zeichentrennzeichen der Textdatei. |
| [SeparatorString](../../aspose.cells/txtloadoptions/separatorstring) { get; set; } | Liest und setzt einen String-Wert als Trennzeichen. |
| [TextQualifier](../../aspose.cells/txtloadoptions/textqualifier) { get; set; } | Gibt den Textbezeichner für Zellenwerte an. Standardkennzeichner ist '''. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells/txtloadoptions/treatconsecutivedelimitersasone) { get; set; } | Ob aufeinanderfolgende Trennzeichen als eins behandelt werden sollen. |
| [TreatQuotePrefixAsValue](../../aspose.cells/txtloadoptions/treatquoteprefixasvalue) { get; set; } | Gibt an, ob das führende einfache Anführungszeichen als Teil des Wertes einer Zelle verwendet werden soll. Der Standardwert ist wahr. Wenn es falsch ist, wird das führende einfache Anführungszeichen aus dem Wert und der entsprechenden Zelle entfernt[`QuotePrefix`](../style/quoteprefix) wird für die Zelle auf true gesetzt. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Ruft Warnrückruf ab oder legt ihn fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Legt das Standarddruckpapierformat aus der Standarddruckereinstellung fest. |

### Siehe auch

* class [AbstractTextLoadOptions](../abstracttextloadoptions)
* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
