---
title: "ChartFrame.IsDefaultPosBeSet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame-egenskap. Anger om standardpositionen DefaultX DefaultY DefaultWidth och DefaultHeight är inställd"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/isdefaultposbeset/
---
## ChartFrame.IsDefaultPosBeSet property

Anger om standardpositionen (DefaultX, DefaultY, DefaultWidth och DefaultHeight) är angiven.

```csharp
public bool IsDefaultPosBeSet { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsDefaultPosBeSetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Bar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till datamärkningar
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Demonstrera IsDefaultPosBeSet-egenskapen
            Console.WriteLine("IsDefaultPosBeSet before setting position: " + dataLabels.IsDefaultPosBeSet);
            
            // Ändra position och kontrollera egenskapen igen
            dataLabels.Position = LabelPositionType.InsideBase;
            Console.WriteLine("IsDefaultPosBeSet after setting position: " + dataLabels.IsDefaultPosBeSet);
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


