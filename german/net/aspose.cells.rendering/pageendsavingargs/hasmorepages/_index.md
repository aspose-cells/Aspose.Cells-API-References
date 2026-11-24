---
title: "PageEndSavingArgs.HasMorePages"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageEndSavingArgs-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob weitere Seiten ausgegeben werden sollen. Der Standardwert ist true"
type: docs
url: /de/net/aspose.cells.rendering/pageendsavingargs/hasmorepages/
---
## PageEndSavingArgs.HasMorePages property

Liest oder setzt einen Wert, der angibt, ob weitere Seiten ausgegeben werden sollen. Der Standardwert ist true.

```csharp
public bool HasMorePages { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageEndSavingArgsPropertyHasMorePagesDemo
    {
        public static void Run()
        {
            // Ein Arbeitsbuch mit Daten erstellen, das sich über mehrere Seiten erstreckt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = $"Row {i + 1}";
            }

            // PDF-Speicheroptionen mit benutzerdefinierter Seitenverarbeitung erstellen
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageControlCallback();

            // Arbeitsbuch mit Seitenbegrenzung speichern
            workbook.Save("PropertyHasMorePagesDemo.pdf", saveOptions);
        }
    }

    internal class PageControlCallback : IPageSavingCallback
    {
        private int pageCount = 0;

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // In dieser Demonstration nicht verwendet
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Lese den aktuellen Eigenschaftswert
            Console.WriteLine($"Page {pageCount} - Initial HasMorePages: {args.HasMorePages}");

            // Eigenschaft nach der ersten Seite ändern
            if (pageCount == 0)
            {
                args.HasMorePages = false;
                Console.WriteLine($"Page {pageCount} - Updated HasMorePages: {args.HasMorePages}");
            }

            pageCount++;
        }
    }
}
```

### Siehe auch

* class [PageEndSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


