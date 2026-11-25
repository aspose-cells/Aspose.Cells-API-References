---
title: "PageSavingArgs.PageIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSavingArgs. Indice della pagina corrente basato su zero"
type: docs
url: /it/net/aspose.cells.rendering/pagesavingargs/pageindex/
---
## PageSavingArgs.PageIndex property

Indice della pagina corrente, basato su zero.

```csharp
public int PageIndex { get; }
```

### Esempi

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
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati al worksheet
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Imposta il callback di salvataggio della pagina
            options.PageSavingCallback = new PageSavingCallback();

            // Salva la cartella di lavoro in PDF - questo attiverà il callback per ogni pagina
            workbook.Save("output.pdf", options);
        }
    }

    public class PageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Dimostra l'uso della proprietà PageIndex
            Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Non utilizzato in questo esempio
        }
    }
}
```

### Vedi anche

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


