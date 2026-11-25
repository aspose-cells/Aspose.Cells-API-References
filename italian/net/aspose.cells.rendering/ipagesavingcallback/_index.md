---
title: "Interfaccia IPageSavingCallback"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Rendering.IPageSavingCallback interfaccia. Controlla/Indica l'avanzamento del processo di salvataggio della pagina"
type: docs
url: /it/net/aspose.cells.rendering/ipagesavingcallback/
---
## IPageSavingCallback interface

Controlla/Indica l'avanzamento del processo di salvataggio della pagina.

```csharp
public interface IPageSavingCallback
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [PageEndSaving](../../aspose.cells.rendering/ipagesavingcallback/pageendsaving/)(PageEndSavingArgs) | Controlla/Indica la fine di una pagina da emettere. |
| [PageStartSaving](../../aspose.cells.rendering/ipagesavingcallback/pagestartsaving/)(PageStartSavingArgs) | Controlla/Indica l'inizio di una pagina da emettere. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageSavingCallbackDemo : IPageSavingCallback
    {
        public static void PageSavingCallbackExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Crea opzioni di salvataggio con una callback di salvataggio della pagina
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.PageSavingCallback = new PageSavingCallbackDemo();

            // Salva la cartella di lavoro come file DOCX
            workbook.Save("PageSavingCallbackExample.docx", saveOptions);
        }

        // Implementa il metodo PageStartSaving
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }

        // Implementa il metodo PageEndSaving
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


