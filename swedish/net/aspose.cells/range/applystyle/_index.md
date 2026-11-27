---
title: "Range.ApplyStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Tillämpar format för ett helt range"
type: docs
url: /sv/net/aspose.cells/range/applystyle/
---
## Range.ApplyStyle method

Tillämpar format för ett helt område.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | Stilobjektet som kommer att tillämpas. |
| flagga | StyleFlag | Flaggor som indikerar tillämpade formateringsegenskaper. |

### Anmärkningar

Varje cell i detta range kommer att innehålla ett [`Style`](../../style/)‑objekt. Så detta är en minneskrävande metod. Använd den försiktigt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;

            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue("Sample text for style demonstration");

            Aspose.Cells.Range range = cells.CreateRange(0, 0, 1, 3);

            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HorizontalAlignment = true;
            styleFlag.VerticalAlignment = true;
            styleFlag.WrapText = true;

            range.ApplyStyle(style, styleFlag);

            workbook.Save("ApplyStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


