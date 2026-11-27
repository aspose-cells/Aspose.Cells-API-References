---
title: "Enum WeightType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.WeightType-enum. Enumererar vikttyperna för en bildram eller en diagramlinje"
type: docs
url: /sv/net/aspose.cells.drawing/weighttype/
---
## WeightType enumeration

Enumererar vikttyperna för en bildram eller en diagramlinje.

```csharp
public enum WeightType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| HairLine | `-1` | Representerar vikten för en hårfin linje. |
| MediumLine | `1` | Representerar vikten för en medelstor linje. |
| SingleLine | `0` | Representerar vikten för en enkel linje. |
| WideLine | `2` | Representerar vikten för en bred linje. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassWeightTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ett diagram och hämta dess diagramområde
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            ChartArea chartArea = chart.ChartArea;
            
            // Ställ in kantens vikt typ
            chartArea.Border.Weight = WeightType.WideLine;
            
            // Verifiera vikttypen
            Console.WriteLine("Chart Area Border Weight: " + chartArea.Border.Weight);
            
            // Spara arbetsboken
            workbook.Save("WeightTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


