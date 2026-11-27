---
title: "WorkbookRender.GetPageSizeInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookRender-metod. Hämtar sidstorlek i tum för utdatabilden"
type: docs
url: /sv/net/aspose.cells.rendering/workbookrender/getpagesizeinch/
---
## WorkbookRender.GetPageSizeInch method

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

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test page size");
            sheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            WorkbookRender wr = new WorkbookRender(wb, imgOpt);
            
            float[] pageSize = wr.GetPageSizeInch(0);
            Console.WriteLine($"Page size in inches: {pageSize[0]} x {pageSize[1]}");
        }
    }
}
```

### Se även

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


