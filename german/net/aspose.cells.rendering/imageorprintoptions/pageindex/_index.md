---
title: "ImageOrPrintOptions.PageIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Gibt den nullbasierten Index der ersten zu speichernden Seite zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/pageindex/
---
## ImageOrPrintOptions.PageIndex property

Liest oder legt den nullbasierten Index der ersten zu speichernden Seite fest.

```csharp
public int PageIndex { get; set; }
```

### Hinweise

Standard ist 0.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zu mehreren Seiten hinzufügen
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
            }

            // Bild-/Druckoptionen einrichten
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PageIndex = 1; // Start from second page (0-based index would be 1)
            options.PageCount = 1; // Only process one page

            // Erstelle SheetRender für das erste Arbeitsblatt
            SheetRender render = new SheetRender(worksheet, options);

            // Mit der richtigen API-Methode als PDF speichern
            render.ToImage(0, "output.pdf");
            Console.WriteLine("Saved page 2 to PDF successfully.");
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


