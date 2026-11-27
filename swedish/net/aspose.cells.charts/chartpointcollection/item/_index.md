---
title: "ChartPointCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPointCollection-egenskap. Hämtar ChartPoint-elementet på det angivna indexet i serien"
type: docs
url: /sv/net/aspose.cells.charts/chartpointcollection/item/
---
## ChartPointCollection indexer

Hämtar [`ChartPoint`](../../chartpoint/) elementet på det angivna indexet i serien.

```csharp
public ChartPoint this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Index för diagrampunkten i serien. |

### Returvärde

ChartPoint-objektet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till en specifik diagrampunkt med Item-egenskapen
            ChartPoint point = chart.NSeries[0].Points[1];
            
            // Ändra punktens fyllningsmönster
            point.Area.FillFormat.Pattern = FillPattern.LightHorizontal;

            // Spara arbetsboken
            workbook.Save("ChartPointCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../../chartpoint/)
* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


