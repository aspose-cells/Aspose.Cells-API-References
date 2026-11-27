---
title: "Cells.ApplyColumnStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metoden. Tillämpar format för en hel kolumn"
type: docs
url: /sv/net/aspose.cells/cells/applycolumnstyle/
---
## Cells.ApplyColumnStyle method

Tillämpar format för en hel kolumn.

```csharp
public void ApplyColumnStyle(int column, Style style, StyleFlag flag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindexet. |
| style | Stil | Stilobjektet som kommer att tillämpas. |
| flagga | StyleFlag | Flaggor som indikerar tillämpade formateringsegenskaper. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyColumnStyleWithInt32StyleStyleFlagDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Skapa en stil med kanter
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            // Skapa en stilflagga för att endast tillämpa kanter
            StyleFlag sflag = new StyleFlag();
            sflag.Borders = true;

            // Tillämpa stilen på kolumn 1 (index 0)
            cells.ApplyColumnStyle(0, style, sflag);

            // Spara arbetsboken
            workbook.Save("ApplyColumnStyleOutput.xlsx");
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


