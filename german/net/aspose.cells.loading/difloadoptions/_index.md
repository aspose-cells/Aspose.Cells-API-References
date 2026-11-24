---
title: "Klasse DifLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Loading.DifLoadOptions class. Stellt die Optionen zum Laden einer .dif‑Datei dar."
type: docs
url: /de/net/aspose.cells.loading/difloadoptions/
---
## DifLoadOptions class

Stellt die Optionen zum Laden einer .dif-Datei dar.

```csharp
public class DifLoadOptions : LoadOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [DifLoadOptions](difloadoptions/)() | Die Optionen. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Liest und schreibt die Optionen des automatischen Anpassers (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Überprüft, ob die Daten in der Vorlagendatei gültig sind. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Ob die Beschränkungen der Excel‑Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht, einen Zeichenkettenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB, z. B. über Cell.PutValue(string), eingeben und diese Eigenschaft true ist, erhalten Sie eine Ausnahme. Ist die Eigenschaft false, wird der eingegebene Zeichenkettenwert als Zellenwert akzeptiert, sodass Sie später den vollständigen Zeichenkettenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Dateiformat speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Liest oder setzt die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Liest die Standard-Style-Einstellungen zum Initialisieren von Stilen der Arbeitsmappe. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Liest und setzt einzelne Schriftkonfigurationen. Funktioniert nur für die [`Workbook`](../../aspose.cells/workbook/), die diese [`LoadOptions`](../../aspose.cells/loadoptions/) zum Laden verwendet. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignoriert Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Gibt an, ob nutzlose Formen ignoriert werden. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Liest und setzt den Unterbrechungsmonitor. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Ob die nicht geparsten Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. Standard ist true. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Liest oder setzt die Sprache der Benutzeroberfläche der Arbeitsmappe-Version basierend auf dem Ländercode, mit dem die Datei gespeichert wurde. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Der Daten-Handler zur Verarbeitung von Zellen­daten beim Lesen einer Vorlagendatei. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Der Filter, der angibt, wie Daten geladen werden. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Liest das Ladeformat. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Liest oder setzt den Speichermodus für die geladene Arbeitsmappe. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Gibt an, ob Formeln beim Lesen der Datei geparst werden. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. Der Standardwert ist false. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Liest und setzt das Passwort der Arbeitsmappe. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Gibt an, ob Leerzeichen und Zeilenumbrüche, die zwischen Formel‑Token eingefügt sind, beim Lesen und Schreiben von Formeln erhalten bleiben. Der Standardwert ist false. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Liest oder setzt die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Legt den Standard‑Schriftartnamen fest (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Legt die Standard‑Schriftgröße fest. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Liest oder setzt den Warn‑Callback. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Legt die Standard‑Papiergröße für den Druck aus den Einstellungen des Standard‑Druckers fest. (Vererbt von [`LoadOptions`](../../aspose.cells/loadoptions/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;

    public class LoadingClassDifLoadOptionsDemo
    {
        public static void Run()
        {
            // Erstelle eine DifLoadOptions‑Instanz
            DifLoadOptions loadOptions = new DifLoadOptions();

            // Erstelle eine Arbeitsmappe (unter Verwendung des parameterlosen Konstruktors)
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten festlegen
            worksheet.Cells["A1"].PutValue("Sample DIF Data");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(200);
            worksheet.Cells["A4"].PutValue(300);

            // Formeln berechnen, falls vorhanden
            workbook.CalculateFormula();

            // Arbeitsmappe im DIF-Format speichern
            workbook.Save("DifLoadOptionsOutput.dif", SaveFormat.Dif);

            // Jetzt das Laden der DIF-Datei mit DifLoadOptions demonstrieren
            DifLoadOptions difOptions = new DifLoadOptions();
            
            // Die gespeicherte DIF-Datei mit den Optionen laden
            Workbook loadedWorkbook = new Workbook("DifLoadOptionsOutput.dif", difOptions);

            // Auf Daten aus der geladenen Arbeitsmappe zugreifen
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            string loadedValue = loadedWorksheet.Cells["A1"].StringValue;

            // Die geladenen Daten zur Überprüfung als XLSX speichern
            loadedWorkbook.Save("DifLoadOptionsVerification.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [LoadOptions](../../aspose.cells/loadoptions/)
* namespace [Aspose.Cells.Loading](../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../)


