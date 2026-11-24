---
title: "WorkbookPrintingPreview.WorkbookPrintingPreview"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookPrintingPreview-Konstruktor. Der Aufbau von WorkbookPrintingPreview"
type: docs
url: /de/net/aspose.cells.rendering/workbookprintingpreview/workbookprintingpreview/
---
## WorkbookPrintingPreview constructor

Der Aufbau von WorkbookPrintingPreview

```csharp
public WorkbookPrintingPreview(Workbook workbook, ImageOrPrintOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Arbeitsmappe | Arbeitsmappe | Geben Sie an, welche Arbeitsmappe gedruckt werden soll. |
| Optionen | ImageOrPrintOptions | ImageOrPrintOptions enthält einige Eigenschaften der Ausgabe |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookPrintingPreviewMethodCtorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Printing Preview");
            
            // Druckoptionen festlegen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintingPage = PrintingPageType.Default;

            // Druckvorschau mit Arbeitsmappe und Optionen erstellen
            WorkbookPrintingPreview preview = new WorkbookPrintingPreview(workbook, options);
            
            // Seitenanzahl anzeigen
            Console.WriteLine("Total pages: " + preview.EvaluatedPageCount);
        }
    }
}
```

### Siehe auch

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


