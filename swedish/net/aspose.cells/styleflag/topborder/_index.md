---
title: "StyleFlag.TopBorder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag egenskap. Inställningar för överkant kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/topborder/
---
## StyleFlag.TopBorder property

Inställningarna för övre kantlinje kommer att tillämpas.

```csharp
public bool TopBorder { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyTopBorderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa en stil med inställningar för överkant
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Dashed;

            // Skapa stilflagga och aktivera modifiering av överkant
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TopBorder = true;

            // Applicera stilen på cell A1 med endast överkant-flagga aktiverad
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Text");
            cell.SetStyle(style, styleFlag);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


