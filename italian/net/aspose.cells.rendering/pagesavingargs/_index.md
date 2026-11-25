---
title: "Classe PageSavingArgs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.PageSavingArgs. Informazioni sul processo di salvataggio di una pagina"
type: docs
url: /it/net/aspose.cells.rendering/pagesavingargs/
---
## PageSavingArgs class

Informazioni per il processo di salvataggio di una pagina.

```csharp
public class PageSavingArgs
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Conteggio totale delle pagine. |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Indice della pagina corrente, basato su zero. |

### Esempi

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
            // Crea una nuova cartella di lavoro con dati estesi per più pagine
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola il foglio di lavoro per generare più pagine durante il rendering
            for (int row = 0; row < 150; row++)
            {
                worksheet.Cells[row, 0].Value = $"Row {row + 1} data";
            }

            // Configura le opzioni di salvataggio PDF con callback di salvataggio pagina
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PageSavingCallback = new PageSavingCallback();

            // Salva la cartella di lavoro in formato PDF con impaginazione
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
                // Opzionale: Aggiungi qui eventuali elaborazioni di fine pagina
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


