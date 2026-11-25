---
title: "PageStartSavingArgs.IsToOutput"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageStartSavingArgs. Ottiene o imposta un valore che indica se la pagina deve essere esportata. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells.rendering/pagestartsavingargs/istooutput/
---
## PageStartSavingArgs.IsToOutput property

Ottiene o imposta un valore che indica se la pagina deve essere esportata. Il valore predefinito è true.

```csharp
public bool IsToOutput { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageStartSavingArgsPropertyIsToOutputDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola i dati per creare più pagine
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
                // Corretto: accedere all'altezza della riga tramite la collezione Rows del foglio di lavoro
                worksheet.Cells.Rows[i].Height = 50;
            }

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new CustomPageSavingCallback();

            workbook.Save("PageOutputDemo.pdf", saveOptions);
        }

        private class CustomPageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Leggi il valore corrente
                Console.WriteLine($"Page {args.PageIndex + 1} - Initial IsToOutput: {args.IsToOutput}");

                // Salta ogni pagina pari (numerazione a partire da 1)
                if ((args.PageIndex + 1) % 2 == 0)
                {
                    args.IsToOutput = false;
                    Console.WriteLine($"Disabling output for page {args.PageIndex + 1}");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Implementazione non necessaria per questa dimostrazione
            }
        }
    }
}
```

### Vedi anche

* class [PageStartSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


