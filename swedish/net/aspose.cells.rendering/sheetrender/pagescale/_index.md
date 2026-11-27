---
title: "SheetRender.PageScale"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SheetRender egenskap. Hämtar beräknad sidskala för bladet. Returnerar den angivna skalan om Zoom är inställd. Annars returneras den beräknade skalan enligt FitToPagesWide och FitToPagesTall"
type: docs
url: /sv/net/aspose.cells.rendering/sheetrender/pagescale/
---
## SheetRender.PageScale property

Hämtar beräknad sidskala för bladet. Returnerar den angivna skalan om [`Zoom`](../../../aspose.cells/pagesetup/zoom/) är inställd. Annars returneras den beräknade skalan enligt [`FitToPagesWide`](../../../aspose.cells/pagesetup/fittopageswide/) och [`FitToPagesTall`](../../../aspose.cells/pagesetup/fittopagestall/).

```csharp
public double PageScale { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderPropertyPageScaleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till exempeldata i celler
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue($"Item {i + 1}");
                sheet.Cells[i, 1].PutValue((i + 1) * 10);
            }

            // Skapa bild- eller utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Skapa bladrendering
            SheetRender sheetRender = new SheetRender(sheet, options);
            
            // Hämta och visa den beräknade sidskalan
            double pageScale = sheetRender.PageScale;
            Console.WriteLine($"Calculated Page Scale: {pageScale}");
        }
    }
}
```

### Se även

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


