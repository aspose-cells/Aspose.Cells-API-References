---
title: "IPageSavingCallback.PageEndSaving"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IPageSavingCallback-metod. Styr/indikera att en sida avslutas för att skrivas ut"
type: docs
url: /sv/net/aspose.cells.rendering/ipagesavingcallback/pageendsaving/
---
## IPageSavingCallback.PageEndSaving method

Styr/indikera att en sida avslutas för utskrift.

```csharp
public void PageEndSaving(PageEndSavingArgs args)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| args | PageEndSavingArgs | Information för en sida avslutar sparprocessen. |

### Exempel

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
            // Skapa en ny arbetsbok och fyll i data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för att skapa flera sidor vid rendering
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[$"A{i+1}"].Value = $"Row {i+1} - Demonstration data for page splitting";
            }

            // Skapa PDF‑spara‑alternativ med anpassad callback för sidsparning
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageEndSavingCallback();

            try
            {
                // Spara arbetsbok med callback‑implementation
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
                // Visa information om slutförd sidsparning
                Console.WriteLine($"Finished processing page {args.PageIndex + 1}");
                
                // Du kan lägga till filoperationer eller annan efterbehandling här
                // args.HasMorePages visar om fler sidor kommer att bearbetas
            }

            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Krävd gränssnittimplementering
            }
        }
    }
}
```

### Se även

* class [PageEndSavingArgs](../../pageendsavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


