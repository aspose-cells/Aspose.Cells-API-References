---
title: "Klasse AutoFitterOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.AutoFitterOptions Klasse. Stellt alle Auto-Fitter-Optionen dar"
type: docs
url: /de/net/aspose.cells/autofitteroptions/
---
## AutoFitterOptions class

Stellt alle Auto-Fitter-Optionen dar.

```csharp
public class AutoFitterOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [AutoFitterOptions](autofitteroptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoFitMergedCells](../../aspose.cells/autofitteroptions/autofitmergedcells/) { get; set; } | (**Obsolete.**) Gibt an, ob die Zeilenhöhe automatisch angepasst wird, wenn die Zellen in einer Zeile zusammengeführt werden. Der Standardwert ist false. |
| [AutoFitMergedCellsType](../../aspose.cells/autofitteroptions/autofitmergedcellstype/) { get; set; } | Liest und setzt den Typ der automatischen Anpassung der Zeilenhöhe zusammengeführter Zellen. |
| [AutoFitWrappedTextType](../../aspose.cells/autofitteroptions/autofitwrappedtexttype/) { get; set; } | Liest und setzt den Typ der automatischen Anpassung von umgebrochenem Text. |
| [DefaultEditLanguage](../../aspose.cells/autofitteroptions/defaulteditlanguage/) { get; set; } | Liest oder setzt die Standardsprache für die Bearbeitung. |
| [FormatStrategy](../../aspose.cells/autofitteroptions/formatstrategy/) { get; set; } | Liest und setzt die formatierte Strategie. |
| [ForRendering](../../aspose.cells/autofitteroptions/forrendering/) { get; set; } | Gibt an, ob die Anpassung für Rendering-Zwecke erfolgt. |
| [IgnoreHidden](../../aspose.cells/autofitteroptions/ignorehidden/) { get; set; } | Ignoriert die ausgeblendeten Zeilen/Spalten. |
| [MaxRowHeight](../../aspose.cells/autofitteroptions/maxrowheight/) { get; set; } | Liest und setzt die maximale Zeilenhöhe (in Punkt) beim automatischen Anpassen von Zeilen. |
| [OnlyAuto](../../aspose.cells/autofitteroptions/onlyauto/) { get; set; } | Gibt an, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitterOptionsDemo
    {
        public static void AutoFitterOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and autofitted.");

            Style style = worksheet.Cells["A1"].GetStyle();

            style.IsTextWrapped = true;

            worksheet.Cells["A1"].SetStyle(style);

            // Erstelle einen Bereich A1:B2
            Range range = worksheet.Cells.CreateRange(0, 0, 2, 2);

            // Zellen zusammenführen
            range.Merge();

            // Eine Instanz von AutoFitterOptions erstellen
            AutoFitterOptions options = new AutoFitterOptions
            {
                DefaultEditLanguage = DefaultEditLanguage.English,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                OnlyAuto = true,
                IgnoreHidden = true,
                MaxRowHeight = 50.0,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                ForRendering = true
            };

            // Zeilen automatisch anpassen mit den angegebenen Optionen
            worksheet.AutoFitRows(options);

            // Speichere die Arbeitsmappe
            workbook.Save("AutoFitterOptionsExample.xlsx");
            workbook.Save("AutoFitterOptionsExample.pdf");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


