---
title: "Chart.HeightPercent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Returnerar eller anger höjden på ett 3D‑diagram som en procentandel av diagrambredden mellan 5 och 500 procent"
type: docs
url: /sv/net/aspose.cells.charts/chart/heightpercent/
---
## Chart.HeightPercent property

Returnerar eller anger höjden på ett 3‑D‑diagram som en procentandel av diagrammets bredd (mellan 5 och 500 procent).

```csharp
public int HeightPercent { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyHeightPercentDemo
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

            // Lägg till ett 3D-kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ange HeightPercent‑egenskapen (styr höjden på 3D‑diagrammet som procentandel av diagrambredden)
            chart.HeightPercent = 150; // 150% of chart width

            // Spara arbetsboken
            workbook.Save("ChartHeightPercentDemo.xlsx");

            Console.WriteLine("Chart with HeightPercent 150% created successfully.");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


