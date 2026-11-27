---
title: "StyleFlag.RightBorder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag-egenskap. Inställningar för högra kanten kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/rightborder/
---
## StyleFlag.RightBorder property

Inställningar för högerkant kommer att tillämpas.

```csharp
public bool RightBorder { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyRightBorderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil med kanter
            Style borderStyle = workbook.CreateStyle();
            borderStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            borderStyle.Borders[BorderType.RightBorder].Color = System.Drawing.Color.Red;

            // Skapa en stilflagga och aktivera högra kanten
            StyleFlag borderFlag = new StyleFlag();
            borderFlag.RightBorder = true;

            // Tillämpa stilen på en cell
            Cell cell = worksheet.Cells["B2"];
            cell.SetStyle(borderStyle, borderFlag);

            // Spara arbetsboken
            workbook.Save("RightBorderDemo.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


