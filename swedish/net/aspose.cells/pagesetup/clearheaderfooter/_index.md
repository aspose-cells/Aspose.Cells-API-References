---
title: "PageSetup.ClearHeaderFooter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Rensar inställningarna för sidhuvud och sidfot"
type: docs
url: /sv/net/aspose.cells/pagesetup/clearheaderfooter/
---
## PageSetup.ClearHeaderFooter method

Rensar inställningarna för sidhuvud och sidfot.

```csharp
public void ClearHeaderFooter()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodClearHeaderFooterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in initiala sidhuvuden och sidfötter
            pageSetup.SetHeader(0, "Initial Left Header");
            pageSetup.SetFooter(0, "Initial Left Footer");

            Console.WriteLine("Before ClearHeaderFooter:");
            Console.WriteLine("Header: " + pageSetup.GetHeader(0));
            Console.WriteLine("Footer: " + pageSetup.GetFooter(0));

            // Rensa sidhuvuden och sidfötter
            pageSetup.ClearHeaderFooter();

            Console.WriteLine("\nAfter ClearHeaderFooter:");
            Console.WriteLine("Header: " + (string.IsNullOrEmpty(pageSetup.GetHeader(0)) ? "Cleared" : "Not Cleared"));
            Console.WriteLine("Footer: " + (string.IsNullOrEmpty(pageSetup.GetFooter(0)) ? "Cleared" : "Not Cleared"));

            // Ställ in nya sidhuvuden och sidfötter efter rensning
            pageSetup.SetHeader(0, "New Left Header");
            pageSetup.SetFooter(0, "New Left Footer");

            Console.WriteLine("\nAfter Setting New Values:");
            Console.WriteLine("Header: " + pageSetup.GetHeader(0));
            Console.WriteLine("Footer: " + pageSetup.GetFooter(0));
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


