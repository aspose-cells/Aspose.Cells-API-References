---
title: "Cells.ApplyRowStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Tillämpar format för en hel rad"
type: docs
url: /sv/net/aspose.cells/cells/applyrowstyle/
---
## Cells.ApplyRowStyle method

Tillämpar format för en hel rad.

```csharp
public void ApplyRowStyle(int row, Style style, StyleFlag flag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| style | Stil | Stilobjektet som kommer att tillämpas. |
| flagga | StyleFlag | Flaggor som indikerar tillämpade formateringsegenskaper. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyRowStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa en stil med kanter
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Skapa stilflagga för kanter
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // Applicera stilen på den första raden
            cells.ApplyRowStyle(0, style, styleFlag);

            // Spara arbetsboken
            workbook.Save("ApplyRowStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


