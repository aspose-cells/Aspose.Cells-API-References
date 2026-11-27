---
title: "ChartCollection.AddFloatingChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartCollection-metod. Lägger till ett diagram i samlingen"
type: docs
url: /sv/net/aspose.cells.charts/chartcollection/addfloatingchart/
---
## ChartCollection.AddFloatingChart method

Lägger till ett diagram i samlingen.

```csharp
public int AddFloatingChart(ChartType type, int left, int top, int width, int height)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | ChartType | Diagramtyp |
| vänster | Int32 | x‑offset till hörnet |
| top | Int32 | y‑offset till hörnet |
| bredd | Int32 | Diagrambredden |
| höjd | Int32 | Diagramhöjden |

### Returvärde

[`Chart`](../../chart/) object index.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodAddFloatingChartWithChartTypeInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till flytande diagram med angivna dimensioner
            int chartIndex = sheet.Charts.AddFloatingChart(ChartType.Column, 100, 100, 600, 400);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Lägg till exempeldata i diagrammet
            chart.NSeries.Add("{1,3,2,5}", false);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


