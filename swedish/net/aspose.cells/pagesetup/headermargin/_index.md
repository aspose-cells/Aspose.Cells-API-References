---
title: "PageSetup.HeaderMargin"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar avståndet från sidans överkant till sidhuvudet i centimeter"
type: docs
url: /sv/net/aspose.cells/pagesetup/headermargin/
---
## PageSetup.HeaderMargin property

Representerar avståndet från sidans topp till sidhuvudet, i enheten centimeter.

```csharp
public double HeaderMargin { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Kom åt PageSetup.
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in sidhuvudsmarginal i centimeter
            pageSetup.HeaderMargin = 1.5;

            // Verifiera att sidhuvudsmarginalen har ställts in
            Console.WriteLine("Header Margin: " + pageSetup.HeaderMargin + " cm");

            // Spara arbetsboken
            workbook.Save("HeaderMarginDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


