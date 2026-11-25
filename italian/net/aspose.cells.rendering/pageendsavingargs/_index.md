---
title: "Classe PageEndSavingArgs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.PageEndSavingArgs. Informazioni sul processo di salvataggio della fine di una pagina"
type: docs
url: /it/net/aspose.cells.rendering/pageendsavingargs/
---
## PageEndSavingArgs class

Informazioni per una pagina terminano il processo di salvataggio.

```csharp
public class PageEndSavingArgs : PageSavingArgs
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [HasMorePages](../../aspose.cells.rendering/pageendsavingargs/hasmorepages/) { get; set; } | Ottiene o imposta un valore che indica se ci sono altre pagine da emettere. Il valore predefinito è true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Conteggio totale delle pagine.(Ereditato da [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Indice della pagina corrente, basato su zero.(Ereditato da [`PageSavingArgs`](../pagesavingargs/).) |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageEndSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Crea un'istanza di PdfSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Imposta il callback PageEndSaving
            saveOptions.PageSavingCallback = new PageEndSavingArgsTest();

            // Salva la cartella di lavoro con il callback
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class PageEndSavingArgsTest : IPageSavingCallback
    {
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Implementazione non necessaria per questa demo
        }
    }
}
```

### Vedi anche

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


