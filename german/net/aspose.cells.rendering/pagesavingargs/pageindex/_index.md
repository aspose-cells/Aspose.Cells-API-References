---
title: "PageSavingArgs.PageIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSavingArgs-Eigenschaft. Aktueller Seitenindex, nullbasiert"
type: docs
url: /de/net/aspose.cells.rendering/pagesavingargs/pageindex/
---
## PageSavingArgs.PageIndex property

Aktueller Seitenindex, nullbasiert.

```csharp
public int PageIndex { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSavingArgsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge dem Arbeitsblatt einige Daten hinzu
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // PDF-Speicheroptionen erstellen
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Legen Sie den Seiten-Speicher-Callback fest
            options.PageSavingCallback = new PageSavingCallback();

            // Speichern Sie die Arbeitsmappe als PDF – dies löst den Callback für jede Seite aus
            workbook.Save("output.pdf", options);
        }
    }

    public class PageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Demonstrieren Sie die Verwendung der PageIndex-Eigenschaft
            Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // In diesem Beispiel nicht verwendet
        }
    }
}
```

### Siehe auch

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


