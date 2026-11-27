---
title: "StyleFlag.HorizontalAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag-egenskap. Inställning för horisontell justering kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/horizontalalignment/
---
## StyleFlag.HorizontalAlignment property

Inställning för horisontell justering kommer att tillämpas.

```csharp
public bool HorizontalAlignment { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa exempeldata i celler
            worksheet.Cells["A1"].PutValue("Left Aligned");
            worksheet.Cells["B1"].PutValue("Center Aligned");
            worksheet.Cells["C1"].PutValue("Right Aligned");
            
            // Skapa stilar med olika horisontella justeringar
            Style styleLeft = workbook.CreateStyle();
            styleLeft.HorizontalAlignment = TextAlignmentType.Left;
            
            Style styleCenter = workbook.CreateStyle();
            styleCenter.HorizontalAlignment = TextAlignmentType.Center;
            
            Style styleRight = workbook.CreateStyle();
            styleRight.HorizontalAlignment = TextAlignmentType.Right;
            
            // Skapa stilflaggor för att endast tillämpa horisontell justering
            StyleFlag flag = new StyleFlag();
            flag.HorizontalAlignment = true;
            
            // Tillämpa stilar på områden
            Aspose.Cells.Range rangeLeft = worksheet.Cells.CreateRange("A1:A1");
            rangeLeft.ApplyStyle(styleLeft, flag);
            
            Aspose.Cells.Range rangeCenter = worksheet.Cells.CreateRange("B1:B1");
            rangeCenter.ApplyStyle(styleCenter, flag);
            
            Aspose.Cells.Range rangeRight = worksheet.Cells.CreateRange("C1:C1");
            rangeRight.ApplyStyle(styleRight, flag);
            
            // Spara arbetsboken
            workbook.Save("HorizontalAlignmentDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


