---
title: "Gränssnitt IPageSavingCallback"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.IPageSavingCallback-gränssnitt. Styr/indikera framsteg för sidlagringsprocessen"
type: docs
url: /sv/net/aspose.cells.rendering/ipagesavingcallback/
---
## IPageSavingCallback interface

Styr/indikera framsteg för sidlagringsprocessen.

```csharp
public interface IPageSavingCallback
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [PageEndSaving](../../aspose.cells.rendering/ipagesavingcallback/pageendsaving/)(PageEndSavingArgs) | Styr/indikera att en sida avslutas för utskrift. |
| [PageStartSaving](../../aspose.cells.rendering/ipagesavingcallback/pagestartsaving/)(PageStartSavingArgs) | Styr/indikera att en sida påbörjas för utskrift. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Skapa sparalternativ med en sidlagringsåteruppringning
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.PageSavingCallback = new PageSavingCallbackDemo();

            // Spara arbetsboken som en DOCX-fil
            workbook.Save("PageSavingCallbackExample.docx", saveOptions);
        }

        // Implementera metoden PageStartSaving
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }

        // Implementera metoden PageEndSaving
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


