---
title: "Style.HorizontalAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style property. Hämtar eller anger den horisontella justeringstypen för texten i en cell"
type: docs
url: /sv/net/aspose.cells/style/horizontalalignment/
---
## Style.HorizontalAlignment property

Hämtar eller anger den horisontella justeringstypen för texten i en cell.

```csharp
public TextAlignmentType HorizontalAlignment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ange text i celler
            cells["A1"].PutValue("Left Aligned");
            cells["A2"].PutValue("Center Aligned");
            cells["A3"].PutValue("Right Aligned");

            // Hämta stilobjekt
            Style styleLeft = cells["A1"].GetStyle();
            Style styleCenter = cells["A2"].GetStyle();
            Style styleRight = cells["A3"].GetStyle();

            // Ange horisontell justering
            styleLeft.HorizontalAlignment = TextAlignmentType.Left;
            styleCenter.HorizontalAlignment = TextAlignmentType.Center;
            styleRight.HorizontalAlignment = TextAlignmentType.Right;

            // Tillämpa stilar på celler
            cells["A1"].SetStyle(styleLeft);
            cells["A2"].SetStyle(styleCenter);
            cells["A3"].SetStyle(styleRight);

            // Spara arbetsboken
            workbook.Save("HorizontalAlignmentDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


