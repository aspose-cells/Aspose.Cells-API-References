---
title: "Klasse TxtLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.TxtLoadOptions Klasse. Stellt die Optionen zum Laden einer Textdatei dar"
type: docs
url: /de/net/aspose.cells/txtloadoptions/
---
## TxtLoadOptions class

Stellt die Optionen zum Laden einer Textdatei dar.

```csharp
public class TxtLoadOptions : AbstractTextLoadOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TxtLoadOptions](txtloadoptions/#constructor)() | Erstellt die Optionen zum Laden einer Textdatei. |
| [TxtLoadOptions](txtloadoptions/#constructor_1)(LoadFormat) | Erstellt die Optionen zum Laden einer Textdatei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Liest und setzt die Auto-Fitter-Optionen.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Prüft, ob die Daten in der Vorlagendatei gültig sind.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Ob die Beschränkungen der Excel-Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenkettenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB über Cell.PutValue(string) eingeben und diese Eigenschaft true ist, erhalten Sie eine Ausnahme. Ist die Eigenschaft false, wird der eingegebene Zeichenkettenwert als Zellenwert akzeptiert, sodass Sie später den vollständigen Zeichenkettenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel-Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel-Format speichern. Andernfalls kann ein unerwarteter Fehler in der erzeugten Excel-Datei auftreten.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Zeichenkette in einer Textdatei in Datumsdaten konvertiert wird. Der Standardwert ist true. (Vererbt von [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Zeichenkette in der Textdatei in numerische Daten konvertiert wird. Standardwert ist true.(Vererbt von [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Liest oder setzt die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Liest die Standard-Style-Einstellungen zum Initialisieren der Stile der Arbeitsmappe.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Liest und setzt die Standardkodierung. Gilt nur für CSV‑Dateien.(Vererbt von [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ExtendToNextSheet](../../aspose.cells/txtloadoptions/extendtonextsheet/) { get; set; } | Ob Daten auf das nächste Blatt erweitert werden, wenn die Zeilen oder Spalten die Grenze überschreiten. Standard ist false. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Liest und setzt einzelne Schriftkonfigurationen. Funktioniert nur für die [`Workbook`](../workbook/), die diese [`LoadOptions`](../loadoptions/) zum Laden verwendet.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/txtloadoptions/hasformula/) { get; set; } | Gibt an, ob der Text eine Formel ist, wenn er mit "=" beginnt. |
| [HasTextQualifier](../../aspose.cells/txtloadoptions/hastextqualifier/) { get; set; } | Ob ein Textqualifizierer für den Zellenwert vorhanden ist. Standard ist true. |
| [HeaderColumnsCount](../../aspose.cells/txtloadoptions/headercolumnscount/) { get; set; } | Die Anzahl der Kopfzeilen-Spalten, die für erweiterte Blätter wiederholt werden. |
| [HeaderRowsCount](../../aspose.cells/txtloadoptions/headerrowscount/) { get; set; } | Die Anzahl der Kopfzeilen-Zeilen, die für erweiterte Blätter wiederholt werden. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignoriere die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Gibt an, ob nutzlose Formen ignoriert werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Liest und setzt den Unterbrechungsmonitor.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [IsMultiEncoded](../../aspose.cells/txtloadoptions/ismultiencoded/) { get; set; } | True bedeutet, dass die Datei mehrere Kodierungen enthält. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Gibt an, ob ein Zeichenkettenwert nicht geparst wird, wenn die Länge 15 beträgt.(Vererbt von [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Ob die nicht geparsten Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. Standard ist true.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Liest oder setzt die Sprache der Benutzeroberfläche der Arbeitsmappen-Version basierend auf dem CountryCode, mit dem die Datei gespeichert wurde.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Der Daten-Handler zur Verarbeitung von Zellen-Daten beim Lesen der Vorlagendatei.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Der Filter, der angibt, wie Daten geladen werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Liest das Ladeformat.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Gibt die Strategie an, die Formatierung für geparste Werte anzuwenden, wenn Zeichenkettenwerte in Zahlen oder Datums‑/Uhrzeitwerte konvertiert werden.(Vererbt von [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MaxColumnCount](../../aspose.cells/txtloadoptions/maxcolumncount/) { get; set; } | Die maximale Anzahl von Spalten, die für ein Blatt importiert werden können. |
| [MaxRowCount](../../aspose.cells/txtloadoptions/maxrowcount/) { get; set; } | Die maximale Anzahl von Zeilen, die für ein Blatt importiert werden können. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Liest oder setzt den Speichermodus für die geladene Arbeitsmappe.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Gibt an, ob die Formel beim Lesen der Datei geparst wird.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. Der Standardwert ist false.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Liest und setzt das Passwort der Arbeitsmappe.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [PreferredParsers](../../aspose.cells/txtloadoptions/preferredparsers/) { get; set; } | Liest und setzt bevorzugte Wertparser zum Laden einer Textdatei. |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Gibt an, ob die zwischen Formeltoken eingefügten Leerzeichen und Zeilenumbrüche beim Lesen und Schreiben von Formeln erhalten bleiben. Der Standardwert ist false.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Liest oder setzt die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [Separator](../../aspose.cells/txtloadoptions/separator/) { get; set; } | Liest und setzt das Zeichen-Trennzeichen der Textdatei. |
| [SeparatorString](../../aspose.cells/txtloadoptions/separatorstring/) { get; set; } | Liest und setzt einen Zeichenkettenwert als Trennzeichen. |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Legt den Standard‑Schriftartnamen fest(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Legt die Standard‑Schriftgröße fest.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [TextQualifier](../../aspose.cells/txtloadoptions/textqualifier/) { get; set; } | Gibt den Textqualifizierer für Zellenwerte an. Standardqualifizierer ist '"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells/txtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | Ob aufeinanderfolgende Trennzeichen als eines behandelt werden sollen. |
| [TreatQuotePrefixAsValue](../../aspose.cells/txtloadoptions/treatquoteprefixasvalue/) { get; set; } | Gibt an, ob das führende einfache Anführungszeichen als Teil des Werts einer Zelle betrachtet werden soll. Standard ist true. Wenn es false ist, wird das führende einfache Anführungszeichen aus dem entsprechenden Zellenwert entfernt und [`QuotePrefix`](../style/quoteprefix/) wird für die Zelle auf true gesetzt. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Liest oder setzt den Warn‑Callback.(Vererbt von [`LoadOptions`](../loadoptions/).) |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Legt die Standard‑Papiergröße des Druckers aus den Druckereinstellungen fest.(Vererbt von [`LoadOptions`](../loadoptions/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class TxtLoadOptionsDemo
    {
        public static void TxtLoadOptionsExample()
        {
            // Erstelle eine Instanz von TxtLoadOptions
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                Separator = ',',
                SeparatorString = ",",
                IsMultiEncoded = false,
                HasFormula = true,
                HasTextQualifier = true,
                TextQualifier = '\"',
                TreatConsecutiveDelimitersAsOne = true,
                TreatQuotePrefixAsValue = true,
                ExtendToNextSheet = false,
                HeaderRowsCount = 1,
                HeaderColumnsCount = 1,
                MaxRowCount = 1000,
                MaxColumnCount = 50,
                Encoding = Encoding.UTF8,
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn,
                ConvertNumericData = true,
                ConvertDateTimeData = true,
                KeepPrecision = true,
                Password = "password",
                ParsingFormulaOnOpen = true,
                ParsingPivotCachedRecords = true,
                LanguageCode = CountryCode.USA,
                Region = CountryCode.USA,
                CultureInfo = new System.Globalization.CultureInfo("en-US"),
                StandardFont = "Arial",
                StandardFontSize = 10.5,
                InterruptMonitor = new InterruptMonitor(),
                IgnoreNotPrinted = true,
                CheckDataValid = true,
                CheckExcelRestriction = true,
                KeepUnparsedData = true,
                LoadFilter = new LoadFilter(LoadDataFilterOptions.All),
                LightCellsDataHandler = new LightCellsDataHandler(),
                MemorySetting = MemorySetting.MemoryPreference,
                WarningCallback = new WarningCallback(),
                AutoFitterOptions = new AutoFitterOptions(),
                AutoFilter = true,
                FontConfigs = new IndividualFontConfigs(),
                IgnoreUselessShapes = true,
                PreservePaddingSpacesInFormula = true
            };

            // Lade eine CSV-Datei mit den angegebenen Optionen
            Workbook workbook = new Workbook("TxtLoadOptionsExample_original.csv", loadOptions);

            // Speichere die Arbeitsmappe in einer Excel‑Datei
            workbook.Save("TxtLoadOptionsExample.xlsx");

            return;
        }
    }

    // Dummy-Implementierungen für referenzierte Klassen/Schnittstellen
    public class InterruptMonitor : AbstractInterruptMonitor
    {
        public override bool IsInterruptionRequested => false;
    }

    public class WarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            Console.WriteLine(warningInfo.Description);
        }
    }

    public class LightCellsDataHandler : Aspose.Cells.LightCellsDataHandler
    {
        public bool StartSheet(Worksheet sheet) => true;
        public bool StartRow(int rowIndex) => true;
        public bool ProcessRow(Row row) => true;
        public bool StartCell(int columnIndex) => true;
        public bool ProcessCell(Cell cell) => true;
    }
}
```

### Siehe auch

* class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


