---
title: "Cells.ApplyStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Tillämpar format för ett helt kalkylblad"
type: docs
url: /sv/net/aspose.cells/cells/applystyle/
---
## Cells.ApplyStyle method

Tillämpar format för ett helt kalkylblad.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | Stilobjektet som kommer att tillämpas. |
| flagga | StyleFlag | Flaggor som indikerar tillämpade formateringsegenskaper. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = wb.Worksheets[0];
            
            // Skapa en stil och aktivera textbrytning
            Style style = wb.CreateStyle();
            style.IsTextWrapped = true;
            
            // Skapa stilflagga och aktivera flagga för textbrytning
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // Tillämpa stilen på alla celler i kalkylbladet
            sheet.Cells.ApplyStyle(style, flag);
            
            // Spara arbetsboken
            wb.Save("output.xlsx", SaveFormat.Xlsx);
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


