---
title: "CellsHelper.GetTextWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper‑metod. Hämta bredden på text i enheten punkter"
type: docs
url: /sv/net/aspose.cells/cellshelper/gettextwidth/
---
## CellsHelper.GetTextWidth method

Hämta textens bredd i enheten punkter.

```csharp
public static double GetTextWidth(string text, Font font, double scaling)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | String | Texten. |
| teckensnitt | Teckensnitt | Teckensnittet för texten. |
| skalning | Double | Skalningen av texten. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetTextWidthWithStringFontDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Font font = workbook.DefaultStyle.Font;
            double textWidth = CellsHelper.GetTextWidth("Sample Text", font, 1.0);
            Console.WriteLine("Text width: " + textWidth);
        }
    }
}
```

### Se även

* class [Font](../../font/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


