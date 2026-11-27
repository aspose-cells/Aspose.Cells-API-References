---
title: "PageSetup.PaperHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Hämtar papperets höjd i enheten tum med hänsyn till sidorientering"
type: docs
url: /sv/net/aspose.cells/pagesetup/paperheight/
---
## PageSetup.PaperHeight property

Hämtar papperets höjd i enheten tum, med hänsyn till sidans orientering.

```csharp
public double PaperHeight { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperHeightDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in data i en cell
            worksheet.Cells["A1"].PutValue("Paper Height Demo");
            
            // Hämta PageSetup-objektet
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Visa standardpappershöjd (i tum)
            Console.WriteLine("Default Paper Height: " + pageSetup.PaperHeight);
            
            // PaperHeight är skrivskyddad, så vi demonstrerar hur man får olika pappersstorlekar
            // genom att ändra pappersstorlekstypen till Letter (8,5x11 tum)
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // Verifiera ändringen
            Console.WriteLine("Modified Paper Height (Letter size): " + pageSetup.PaperHeight);
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


