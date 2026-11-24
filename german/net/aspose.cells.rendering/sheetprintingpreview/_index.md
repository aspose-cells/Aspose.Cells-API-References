---
title: "Klasse SheetPrintingPreview"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.SheetPrintingPreview Klasse. Arbeitsblatt‑Druckvorschau"
type: docs
url: /de/net/aspose.cells.rendering/sheetprintingpreview/
---
## SheetPrintingPreview class

Druckvorschau des Arbeitsblatts.

```csharp
public class SheetPrintingPreview
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SheetPrintingPreview](sheetprintingpreview/)(Worksheet, ImageOrPrintOptions) | Der Aufbau von SheetPrintingPreview |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/sheetprintingpreview/evaluatedpagecount/) { get; } | Ermittele die Gesamtseitenzahl dieses Arbeitsblatts |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetPrintingPreviewDemo
    {
        public static void SheetPrintingPreviewExample()
        {
            // Lade eine vorhandene Arbeitsmappe
            Workbook workbook = new Workbook("SheetPrintingPreviewDemo_original.xlsx");

            // Hole das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Erstelle eine Instanz von SheetPrintingPreview
            SheetPrintingPreview sheetPrintingPreview = new SheetPrintingPreview(worksheet, options);

            // Ermittele und drucke die Gesamtseitenzahl des Arbeitsblatts
            Console.WriteLine("Total Page Count: " + sheetPrintingPreview.EvaluatedPageCount);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


