---
title: "IPageSavingCallback.PageStartSaving"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IPageSavingCallback. Controlla/Indica l'inizio di una pagina da esportare"
type: docs
url: /it/net/aspose.cells.rendering/ipagesavingcallback/pagestartsaving/
---
## IPageSavingCallback.PageStartSaving method

Controlla/Indica l'inizio di una pagina da emettere.

```csharp
public void PageStartSaving(PageStartSavingArgs args)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| args | PageStartSavingArgs | Informazioni per l'avvio del processo di salvataggio di una pagina. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class IPageSavingCallbackMethodPageStartSavingWithPageStartSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi contenuto di esempio per creare più pagine
            for (int i = 0; i < 150; i++)
                worksheet.Cells[$"A{i + 1}"].Value = $"Data row {i + 1}";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PageSavingCallback callback = new PageSavingCallback();
            saveOptions.PageSavingCallback = callback;

            try
            {
                workbook.Save("PageStartSavingOutput.pdf", saveOptions);
                Console.WriteLine($"Processed pages: {callback.ProcessedPages}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class PageSavingCallback : IPageSavingCallback
    {
        public int ProcessedPages { get; private set; }

        public void PageStartSaving(PageStartSavingArgs args)
        {
            if (args.PageIndex % 3 == 0) // Skip every 3rd page (0-based)
                args.IsToOutput = false;
            else
                ProcessedPages++;

            Console.WriteLine(args.IsToOutput 
                ? $"Saving page {args.PageIndex + 1}"
                : $"Skipping page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Gestione opzionale della fine della pagina
        }
    }
}
```

### Vedi anche

* class [PageStartSavingArgs](../../pagestartsavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


