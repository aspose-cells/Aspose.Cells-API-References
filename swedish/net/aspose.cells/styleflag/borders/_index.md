---
title: "StyleFlag.Borders"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag egenskap. Alla kantinställningar kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/borders/
---
## StyleFlag.Borders property

Alla kantinställningar kommer att tillämpas.

```csharp
public bool Borders { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBordersDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa en stil med kantinställningar
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].Color = System.Drawing.Color.Blue;

            // Skapa en stilflagga och aktivera kanter
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // Applicera stilen på cell A1 med endast kanter
            cells["A1"].PutValue("Borders Demo");
            cells["A1"].SetStyle(style, styleFlag);

            // Spara arbetsboken
            workbook.Save("BordersDemo.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


