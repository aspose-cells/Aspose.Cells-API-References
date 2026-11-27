---
title: "PageSetup.IsHFDiffFirst"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup egenskap. Sant betyder att header/footer på den första sidan är annorlunda än på andra sidor"
type: docs
url: /sv/net/aspose.cells/pagesetup/ishfdifffirst/
---
## PageSetup.IsHFDiffFirst property

True betyder att sidhuvudet/sidfoten på den första sidan är annorlunda än på andra sidor.

```csharp
public bool IsHFDiffFirst { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffFirstDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kom åt PageSetup.
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Ställ in olika sidhuvuden/sidfötter för första sidan
            pageSetup.IsHFDiffFirst = true;
            
            // Ställ in header/footer
            pageSetup.SetFirstPageHeader(0, "First Page Header");
            pageSetup.SetHeader(0, "Standard Header");
            
            // Spara arbetsboken
            workbook.Save("PageSetup_IsHFDiffFirst_Example.xlsx");
            
            // Läs in arbetsboken på nytt för att verifiera inställningarna
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffFirst_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            // Utskriftsverifiering
            Console.WriteLine("IsHFDiffFirst: " + loadedPageSetup.IsHFDiffFirst);
            Console.WriteLine("First Page Header: " + loadedPageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Standard Header: " + loadedPageSetup.GetHeader(0));
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


