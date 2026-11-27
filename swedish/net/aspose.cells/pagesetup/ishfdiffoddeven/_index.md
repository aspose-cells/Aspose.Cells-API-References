---
title: "PageSetup.IsHFDiffOddEven"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. True betyder att sidhuvudet/sidfoten för udda sidor är olika med udda sidor"
type: docs
url: /sv/net/aspose.cells/pagesetup/ishfdiffoddeven/
---
## PageSetup.IsHFDiffOddEven property

True betyder att sidhuvudet/sidfoten på udda sidor är annorlunda än på udda sidor.

```csharp
public bool IsHFDiffOddEven { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffOddEvenDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kom åt PageSetup.
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Aktivera olika sidhuvuden/sidfötter för udda och jämna sidor
            pageSetup.IsHFDiffOddEven = true;
            
            // Ställ in olika sidfötter för udda och jämna sidor
            pageSetup.SetFooter(0, "Odd Page Footer");
            pageSetup.SetEvenFooter(0, "Even Page Footer");
            
            // Spara arbetsboken
            workbook.Save("PageSetup_IsHFDiffOddEven_Example.xlsx");
            
            // Verifiera inställningarna genom att ladda den sparade filen
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffOddEven_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            Console.WriteLine("IsHFDiffOddEven: " + loadedPageSetup.IsHFDiffOddEven);
            Console.WriteLine("Odd Page Footer: " + loadedPageSetup.GetFooter(0));
            Console.WriteLine("Even Page Footer: " + loadedPageSetup.GetEvenFooter(0));
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


