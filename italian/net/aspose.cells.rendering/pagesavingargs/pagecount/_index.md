---
title: "PageSavingArgs.PageCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSavingArgs. Conteggio totale delle pagine"
type: docs
url: /it/net/aspose.cells.rendering/pagesavingargs/pagecount/
---
## PageSavingArgs.PageCount property

Conteggio totale delle pagine.

```csharp
public int PageCount { get; }
```

### Esempi

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
            // Crea un nuovo workbook e aggiungi dati di test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi contenuto denso per creare più pagine
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // Imposta la configurazione della pagina per controllare l'impaginazione
            worksheet.PageSetup.PrintArea = "A1:A50";
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // Crea opzioni di salvataggio PDF con callback di salvataggio pagina
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new PageSavingCallback();

            // Salva in PDF per attivare l'impaginazione
            workbook.Save("PageSavingDemo.pdf", options);
        }

        private class PageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Accedi a PageCount dagli argomenti dell'evento
                Console.WriteLine($"Saving page {args.PageIndex + 1} of {args.PageCount}");
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Nessuna implementazione necessaria
            }
        }
    }
}
```

### Vedi anche

* class [PageSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


