---
title: "PageSetup.FooterMargin"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup egenskap. Representerar avståndet från sidans botten till sidfoten i enheten centimeter"
type: docs
url: /sv/net/aspose.cells/pagesetup/footermargin/
---
## PageSetup.FooterMargin property

Representerar avståndet från sidans botten till sidfoten, i enheten centimeter.

```csharp
public double FooterMargin { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Kom åt PageSetup.
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in sidfotens marginal i centimeter
            pageSetup.FooterMargin = 1.5;

            // Lägg till lite innehåll för att se effekten
            worksheet.Cells["A1"].PutValue("Footer Margin Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates setting footer margin to 1.5 cm");

            // Ställ in sidfotstext för att göra marginalen synlig
            pageSetup.SetFooter(0, "&A - Footer text to demonstrate margin");

            // Spara arbetsboken
            workbook.Save("FooterMarginDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


