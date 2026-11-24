---
title: "Klasse LoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LoadOptions‑Klasse. Stellt die Optionen zum Laden der Datei dar"
type: docs
url: /de/net/aspose.cells/loadoptions/
---
## LoadOptions class

Stellt die Optionen für das Laden der Datei dar.

```csharp
public class LoadOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [LoadOptions](loadoptions/#constructor)() | Erstellt eine Option zum Laden der Datei. |
| [LoadOptions](loadoptions/#constructor_1)(LoadFormat) | Erstellt eine Option zum Laden der Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Liest und legt die Auto‑Fitter‑Optionen fest |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Überprüft, ob die Daten in der Vorlagendatei gültig sind. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Ob die Beschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht, einen Zeichenfolgenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K eingeben, etwa mit Cell.PutValue(string), erhalten Sie bei true dieser Eigenschaft eine Exception. Ist die Eigenschaft false, akzeptieren wir Ihren Eingabestring als Zellwert, sodass Sie später den vollständigen Zeichenfolgenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel-Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel-Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel-Datei kommen. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Liest oder legt die regionalen Einstellungen fest, die für die zu ladende Arbeitsmappe verwendet werden. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Liest die Standard‑Stil‑Einstellungen zum Initialisieren der Stile der Arbeitsmappe. |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Liest und legt einzelne Schriftkonfigurationen fest. Funktioniert nur für die [`Workbook`](../workbook/), die diese `LoadOptions` zum Laden verwendet. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignoriere die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird. |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Gibt an, ob nutzlose Formen ignoriert werden sollen. |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Liest und setzt den Interrupt‑Monitor. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Ob die nicht geparsten Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. Standard ist true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Liest oder setzt die Benutzeroberflächensprache der Workbook-Version basierend auf dem CountryCode, das die Datei gespeichert hat. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Der Datenhandler zur Verarbeitung von Zellen­daten beim Lesen der Vorlagendatei. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Der Filter, der angibt, wie Daten geladen werden. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Liest das Ladeformat. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Liest oder legt den Speichermodus für die geladene Arbeitsmappe fest. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Gibt an, ob Formeln beim Lesen der Datei geparst werden. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. Der Standardwert ist false. |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Liest und legt das Passwort der Arbeitsmappe fest. |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Gibt an, ob Leerzeichen und Zeilenumbrüche, die zwischen Formeltoken eingefügt sind, beim Lesen und Schreiben von Formeln erhalten bleiben sollen. Der Standardwert ist false. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Liest oder legt die regionalen Einstellungen fest, die für die zu ladende Arbeitsmappe verwendet werden. |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Setzt den Standard‑Schriftartnamen |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Setzt die Standard‑Schriftgröße. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Liest oder setzt den Warnungs-Callback. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Setzt die Standard‑Papiergröße für den Druck aus den Einstellungen des Standard‑Druckers. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class LoadOptionsDemo
    {
        public static void LoadOptionsExample()
        {
            // Erstelle eine Instanz von LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Eigenschaften festlegen
            loadOptions.Password = "password123";
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = false;
            loadOptions.LanguageCode = CountryCode.USA;
            loadOptions.Region = CountryCode.USA;
            loadOptions.CultureInfo = new CultureInfo("en-US");
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = false;
            loadOptions.KeepUnparsedData = true;
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            loadOptions.AutoFitterOptions = new AutoFitterOptions { AutoFitMergedCells = true };
            loadOptions.AutoFilter = true;
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = false;

            // Laden Sie eine Arbeitsmappe mit den angegebenen LoadOptions.
            Workbook workbook = new Workbook("LoadOptionsExample_original.xlsx", loadOptions);

            // Führe Operationen auf der Arbeitsmappe aus
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, World!");

            // Speichere die Arbeitsmappe
            workbook.Save("LoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


