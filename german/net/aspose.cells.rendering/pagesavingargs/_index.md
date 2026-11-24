---
title: "Klasse PageSavingArgs"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.PageSavingArgs Klasse. Informationen zum Seiten‑Speichervorgang"
type: docs
url: /de/net/aspose.cells.rendering/pagesavingargs/
---
## PageSavingArgs class

Info für einen Seiten‑Speichervorgang.

```csharp
public class PageSavingArgs
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Gesamtseitenzahl. |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Aktueller Seitenindex, nullbasiert. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassPageSavingArgsDemo
    {
        public static void Run()
        {
            // Ein neues Arbeitsbuch mit erweiterten Daten für mehrere Seiten erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Arbeitsblatt füllen, um beim Rendern mehrere Seiten zu erzeugen
            for (int row = 0; row < 150; row++)
            {
                worksheet.Cells[row, 0].Value = $"Row {row + 1} data";
            }

            // PDF‑Speicheroptionen mit Seiten‑Speicher‑Callback konfigurieren
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PageSavingCallback = new PageSavingCallback();

            // Arbeitsbuch im PDF-Format mit Seitennummerierung speichern
            workbook.Save("RenderingPageSavingDemo.pdf", pdfSaveOptions);
        }

        private class PageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
                
                if (args.PageIndex == 0)
                {
                    Console.WriteLine("Processing cover page...");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Optional: Hier beliebige End‑der‑Seite‑Verarbeitung hinzufügen
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


