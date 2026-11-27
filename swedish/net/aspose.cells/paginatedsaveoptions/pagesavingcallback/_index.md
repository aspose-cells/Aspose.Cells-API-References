---
title: "PaginatedSaveOptions.PageSavingCallback"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions-egenskap. Kontrollera/indikera framsteg för sid sparningsprocessen"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/pagesavingcallback/
---
## PaginatedSaveOptions.PageSavingCallback property

Styr/indikera framsteg för sidlagringsprocessen.

```csharp
public IPageSavingCallback PageSavingCallback { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageSavingCallbackDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            worksheet.Cells["A2"].PutValue("This demonstrates PageSavingCallback");

            // Skapa sparalternativ med återuppringning för sid sparning
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new CustomPageSavingCallback();

            // Spara med återuppringning
            workbook.Save("PageSavingCallbackDemo.pdf", saveOptions);
        }
    }

    public class CustomPageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex + 1}");
            if (args.HasMorePages)
            {
                Console.WriteLine("More pages to follow...");
            }
        }
    }
}
```

### Se även

* interface [IPageSavingCallback](../../../aspose.cells.rendering/ipagesavingcallback/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


