---
title: "Klasse WorkbookPrintingPreview"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.WorkbookPrintingPreview Klasse. Druckvorschau für Arbeitsmappe"
type: docs
url: /de/net/aspose.cells.rendering/workbookprintingpreview/
---
## WorkbookPrintingPreview class

Druckvorschau der Arbeitsmappe.

```csharp
public class WorkbookPrintingPreview
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [WorkbookPrintingPreview](workbookprintingpreview/)(Workbook, ImageOrPrintOptions) | Der Aufbau von WorkbookPrintingPreview |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [EvaluatedPageCount](../../aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/) { get; } | Ermitteln Sie die Gesamtseitenzahl dieser Arbeitsmappe |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class WorkbookPrintingPreviewDemo
    {
        public static void WorkbookPrintingPreviewExample()
        {
            // Lade eine vorhandene Arbeitsmappe
            Workbook workbook = new Workbook("WorkbookPrintingPreviewExample_original.xlsx");

            // Erstelle eine Instanz von ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Eine Instanz von WorkbookPrintingPreview erstellen
            WorkbookPrintingPreview workbookPrintingPreview = new WorkbookPrintingPreview(workbook, options);

            // Ermitteln Sie die Gesamtseitenzahl der Arbeitsmappe
            int pageCount = workbookPrintingPreview.EvaluatedPageCount;

            // Geben Sie die ermittelte Seitenzahl aus
            Console.WriteLine("Total Page Count: " + pageCount);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


