---
title: "StyleFlag.BottomBorder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "StyleFlag-egenskap. Inställningar för nedre kant kommer att tillämpas"
type: docs
url: /sv/net/aspose.cells/styleflag/bottomborder/
---
## StyleFlag.BottomBorder property

Inställningar för bottenkant kommer att tillämpas.

```csharp
public bool BottomBorder { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBottomBorderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa en stil med inställningar för nedre kant
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Red;

            // Skapa stilflagga och aktivera modifiering av nedre kant
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.BottomBorder = true;

            // Applicera stilen med flaggan på cell A1
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Cell with bottom border");
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


