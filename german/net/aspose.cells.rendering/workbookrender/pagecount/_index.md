---
title: "WorkbookRender.PageCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookRender-Eigenschaft. Gibt die Gesamtseitenzahl des Arbeitsbuchs zurück"
type: docs
url: /de/net/aspose.cells.rendering/workbookrender/pagecount/
---
## WorkbookRender.PageCount property

Ermittelt die Gesamtseitenzahl der Arbeitsmappe.

```csharp
public int PageCount { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            
            // Füge ein zweites Arbeitsblatt hinzu
            workbook.Worksheets.Add();
            worksheet = workbook.Worksheets[1];
            worksheet.Cells["A1"].PutValue("Page 2 Content");

            // Render-Optionen und Workbook-Renderer erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };
            
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // Demonstriere die Verwendung von PageCount
            Console.WriteLine($"Total pages to render: {renderer.PageCount}");
            
            // Jede Seite in ein Bild rendern
            for (int i = 0; i < renderer.PageCount; i++)
            {
                string outputPath = $"Page_{i}.png";
                renderer.ToImage(i, outputPath);
                Console.WriteLine($"Rendered page {i+1} to {outputPath}");
            }
        }
    }
}
```

### Siehe auch

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


