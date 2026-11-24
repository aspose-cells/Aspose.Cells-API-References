---
title: "WorkbookPrintingPreview.EvaluatedPageCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookPrintingPreview-Eigenschaft. Ermittelt die Gesamtseitenzahl dieser Arbeitsmappe"
type: docs
url: /de/net/aspose.cells.rendering/workbookprintingpreview/evaluatedpagecount/
---
## WorkbookPrintingPreview.EvaluatedPageCount property

Ermitteln Sie die Gesamtseitenzahl dieser Arbeitsmappe

```csharp
public int EvaluatedPageCount { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookPrintingPreviewPropertyEvaluatedPageCountDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Arbeitsblatt hinzufügen
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].PutValue("Row " + (i + 1));
            }

            // Optionen für die Druckvorschau erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Druckvorschau für Arbeitsmappe erstellen
            WorkbookPrintingPreview printingPreview = new WorkbookPrintingPreview(workbook, options);
            
            // Ermittelt und zeigt die berechnete Seitenzahl an
            Console.WriteLine("Evaluated Page Count: " + printingPreview.EvaluatedPageCount);
        }
    }
}
```

### Siehe auch

* class [WorkbookPrintingPreview](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


