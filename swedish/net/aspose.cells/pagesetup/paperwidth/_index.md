---
title: "PageSetup.PaperWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup egenskap. Hämtar papperets bredd i tum med hänsyn till sidorientering"
type: docs
url: /sv/net/aspose.cells/pagesetup/paperwidth/
---
## PageSetup.PaperWidth property

Hämtar papperets bredd i enheten tum, med hänsyn till sidans orientering.

```csharp
public double PaperWidth { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperWidthDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange några exempeldata
            worksheet.Cells["A1"].PutValue("Sample Page Setup Demo");
            
            // Åtkomst till PageSetup för kalkylbladet
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Demonstrera PaperWidth-egenskapen (endast läsning)
            Console.WriteLine("Paper Width: " + pageSetup.PaperWidth);
            
            // För att ändra papperstorlek, använd PaperSize-egenskapen istället
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            Console.WriteLine("New Paper Width: " + pageSetup.PaperWidth);
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


