---
title: "PageEndSavingArgs.HasMorePages"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageEndSavingArgs. Ottiene o imposta un valore che indica se ci sono altre pagine da emettere. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells.rendering/pageendsavingargs/hasmorepages/
---
## PageEndSavingArgs.HasMorePages property

Ottiene o imposta un valore che indica se ci sono altre pagine da emettere. Il valore predefinito è true.

```csharp
public bool HasMorePages { get; set; }
```

### Esempi

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
            // Crea una cartella di lavoro con dati che si estendono su più pagine
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = $"Row {i + 1}";
            }

            // Crea opzioni di salvataggio PDF con gestione personalizzata delle pagine
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageControlCallback();

            // Salva la cartella di lavoro con limitazione delle pagine
            workbook.Save("PropertyHasMorePagesDemo.pdf", saveOptions);
        }
    }

    internal class PageControlCallback : IPageSavingCallback
    {
        private int pageCount = 0;

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Non utilizzato in questa dimostrazione
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Leggi il valore corrente della proprietà
            Console.WriteLine($"Page {pageCount} - Initial HasMorePages: {args.HasMorePages}");

            // Modifica la proprietà dopo la prima pagina
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

### Vedi anche

* class [PageEndSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


