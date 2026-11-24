---
title: "Klasse JsonLoadOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.JsonLoadOptions Klasse. Stellt die Optionen für das Laden von JSON-Dateien dar"
type: docs
url: /de/net/aspose.cells/jsonloadoptions/
---
## JsonLoadOptions class

Stellt die Optionen für das Laden von JSON-Dateien dar.

```csharp
public class JsonLoadOptions : LoadOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [JsonLoadOptions](jsonloadoptions/)() | Erstellt eine Option zum Laden der Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Gibt an, ob die Daten beim Laden der Dateien automatisch gefiltert werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Liest und setzt die Auto-Fitter-Optionen.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Prüft, ob die Daten in der Vorlagendatei gültig sind.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Ob die Beschränkungen der Excel-Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenkettenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB über Cell.PutValue(string) eingeben und diese Eigenschaft true ist, erhalten Sie eine Ausnahme. Ist die Eigenschaft false, wird der eingegebene Zeichenkettenwert als Zellenwert akzeptiert, sodass Sie später den vollständigen Zeichenkettenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel-Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel-Format speichern. Andernfalls kann ein unerwarteter Fehler in der erzeugten Excel-Datei auftreten.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Liest oder setzt die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | Liest die Standard-Style-Einstellungen zum Initialisieren der Stile der Arbeitsmappe.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Liest und setzt einzelne Schriftkonfigurationen. Funktioniert nur für die [`Workbook`](../workbook/), die diese [`LoadOptions`](../loadoptions/) zum Laden verwendet.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Ignoriere die Daten, die nicht gedruckt werden, wenn die Datei direkt gedruckt wird.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Gibt an, ob nutzlose Formen ignoriert werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Liest und setzt den Unterbrechungsmonitor.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Ob die nicht geparsten Daten im Speicher für die Arbeitsmappe behalten werden, wenn sie aus einer Vorlagendatei geladen wird. Standard ist true.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [KeptSchema](../../aspose.cells/jsonloadoptions/keptschema/) { get; set; } | Gibt an, ob das Schema dieses JSON beibehalten wird. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Liest oder setzt die Sprache der Benutzeroberfläche der Arbeitsmappen-Version basierend auf dem CountryCode, mit dem die Datei gespeichert wurde.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [LayoutOptions](../../aspose.cells/jsonloadoptions/layoutoptions/) { get; set; } | Die Optionen für den JSON-Import. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Der Daten-Handler zur Verarbeitung von Zellen-Daten beim Lesen der Vorlagendatei.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Der Filter, der angibt, wie Daten geladen werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Liest das Ladeformat.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Liest oder setzt den Speichermodus für die geladene Arbeitsmappe.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [MultipleWorksheets](../../aspose.cells/jsonloadoptions/multipleworksheets/) { get; set; } | Gibt an, ob jedes Attribut des JsonObject-Objekts als ein Arbeitsblatt importiert wird, wenn alle Kindknoten Array-Knoten sind. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Gibt an, ob die Formel beim Lesen der Datei geparst wird.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Gibt an, ob Pivot‑Cache‑Datensätze beim Laden der Datei geparst werden. Der Standardwert ist false.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Liest und setzt das Passwort der Arbeitsmappe.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Gibt an, ob die zwischen Formeltoken eingefügten Leerzeichen und Zeilenumbrüche beim Lesen und Schreiben von Formeln erhalten bleiben. Der Standardwert ist false.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Liest oder setzt die regionalen Einstellungen, die für die zu ladende Arbeitsmappe verwendet werden.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Legt den Standard‑Schriftartnamen fest(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Legt die Standard‑Schriftgröße fest.(Vererbt von [`LoadOptions`](../loadoptions/).) |
| [StartCell](../../aspose.cells/jsonloadoptions/startcell/) { get; set; } | Liest und setzt die Startzelle. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Liest oder setzt den Warn‑Callback.(Vererbt von [`LoadOptions`](../loadoptions/).) |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Legt die Standard‑Papiergröße des Druckers aus den Druckereinstellungen fest.(Vererbt von [`LoadOptions`](../loadoptions/).) |

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Utility;
using System;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsDemo
    {
        public static void JsonLoadOptionsExample()
        {
            // Erstelle eine Instanz von JsonLoadOptions
            JsonLoadOptions jsonLoadOptions = new JsonLoadOptions
            {
                StartCell = "A1",
                MultipleWorksheets = true,
                KeptSchema = true,
                LayoutOptions = new JsonLayoutOptions
                {
                    ArrayAsTable = true,
                    IgnoreNull = false,
                    IgnoreTitle = false,
                    ConvertNumericOrDate = true,
                    NumberFormat = "0.00",
                    DateFormat = "yyyy-MM-dd"
                }
            };

            // Lade JSON‑Daten in eine Arbeitsmappe
            string jsonFilePath = "JsonLoadOptionsExample_data.json";
            Workbook workbook = new Workbook(jsonFilePath, jsonLoadOptions);

            // Speichere die Arbeitsmappe in einer Excel‑Datei
            workbook.Save("JsonLoadOptionsExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [LoadOptions](../loadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


