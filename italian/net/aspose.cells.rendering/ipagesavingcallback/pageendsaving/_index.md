---
title: "IPageSavingCallback.PageEndSaving"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IPageSavingCallback. Controlla/Indica la fine di una pagina da esportare"
type: docs
url: /it/net/aspose.cells.rendering/ipagesavingcallback/pageendsaving/
---
## IPageSavingCallback.PageEndSaving method

Controlla/Indica la fine di una pagina da emettere.

```csharp
public void PageEndSaving(PageEndSavingArgs args)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| args | PageEndSavingArgs | Informazioni per una pagina terminano il processo di salvataggio. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class IPageSavingCallbackMethodPageEndSavingWithPageEndSavingArgsDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e popola i dati
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per creare più pagine durante il rendering
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[$"A{i+1}"].Value = $"Row {i+1} - Demonstration data for page splitting";
            }

            // Crea le opzioni di salvataggio PDF con callback personalizzato per il salvataggio delle pagine
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageEndSavingCallback();

            try
            {
                // Salva la cartella di lavoro con l'implementazione del callback
                workbook.Save("PageEndSavingDemo.pdf", saveOptions);
                Console.WriteLine("Document saved successfully with page end tracking.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during document save: {ex.Message}");
            }
        }

        private class PageEndSavingCallback : IPageSavingCallback
        {
            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Visualizza le informazioni di completamento del salvataggio della pagina
                Console.WriteLine($"Finished processing page {args.PageIndex + 1}");
                
                // Puoi aggiungere operazioni di file o altri post‑processi qui
                // args.HasMorePages indica se verranno elaborate altre pagine
            }

            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Implementazione dell'interfaccia richiesta
            }
        }
    }
}
```

### Vedi anche

* class [PageEndSavingArgs](../../pageendsavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


