---
title: "Style.SetPatternColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-metod. Anger bakgrundsfärgen"
type: docs
url: /sv/net/aspose.cells/style/setpatterncolor/
---
## Style.SetPatternColor method

Ställer in bakgrundsfärgen.

```csharp
public void SetPatternColor(BackgroundType pattern, Color color1, Color color2)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mönster | BackgroundType | Mönstret. |
| color1 | Färg | Förgrundsfärgen. |
| color2 | Färg | Bakgrundsfärgen. Fungerar endast när mönstret inte är BackgroundType.None och BackgroundType.Solid. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetPatternColorWithBackgroundTypeColorColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.SetPatternColor(BackgroundType.Solid, Color.Red, Color.Blue);
            cell.SetStyle(style);
            
            workbook.Save("SetPatternColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


