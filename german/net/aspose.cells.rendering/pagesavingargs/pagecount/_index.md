---
title: "PageSavingArgs.PageCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSavingArgs-Eigenschaft. Gesamtseitenzahl"
type: docs
url: /de/net/aspose.cells.rendering/pagesavingargs/pagecount/
---
## PageSavingArgs.PageCount property

Gesamtseitenzahl.

```csharp
public int PageCount { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageSavingArgsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und fügen Sie Testdaten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie dichten Inhalt hinzu, um mehrere Seiten zu erzeugen
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // Legen Sie die Seiteneinrichtung fest, um die Seitennummerierung zu steuern
            worksheet.PageSetup.PrintArea = "A1:A50";
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // PDF-Speicheroptionen mit Seiten-Speicher-Callback erstellen
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new PageSavingCallback();

            // Als PDF speichern, um die Seitennummerierung auszulösen
            workbook.Save("PageSavingDemo.pdf", options);
        }

        private class PageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Greifen Sie auf PageCount aus den Ereignisargumenten zu
                Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Keine Implementierung erforderlich
            }
        }
    }
}
```

### Siehe auch

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


