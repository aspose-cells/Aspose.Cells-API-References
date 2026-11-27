---
title: "SheetRender.GetPageSizeInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SheetRender-metod. Hämta sidstorlek i tum för den utgående bilden"
type: docs
url: /sv/net/aspose.cells.rendering/sheetrender/getpagesizeinch/
---
## SheetRender.GetPageSizeInch method

Hämta sidstorlek i tum för den genererade bilden.

```csharp
public float[] GetPageSizeInch(int pageIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageIndex | Int32 | Sidindexet är baserat på noll. |

### Returvärde

Bildens sidstorlek, [0] för bredd och [1] för höjd

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.PrintArea = "A1:D10";
            worksheet.PageSetup.LeftMargin = 0;
            worksheet.PageSetup.RightMargin = 0;
            worksheet.PageSetup.TopMargin = 0;
            worksheet.PageSetup.BottomMargin = 0;

            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true,
                ImageType = ImageType.Png
            };

            SheetRender sheetRender = new SheetRender(worksheet, options);
            float[] pageSize = sheetRender.GetPageSizeInch(0);
            
            Console.WriteLine($"Page Size (Inches): Width={pageSize[0]}, Height={pageSize[1]}");
        }
    }
}
```

### Se även

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


