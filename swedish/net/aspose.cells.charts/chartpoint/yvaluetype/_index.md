---
title: "ChartPoint.YValueType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint egenskap. Hämtar Y‑värdetypen för diagrampunkten."
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/yvaluetype/
---
## ChartPoint.YValueType property

Hämtar Y‑värdestypen för diagrampunkten.

```csharp
public CellValueType YValueType { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyYValueTypeDemo
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

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta den första diagrampunkten i den första serien
            ChartPoint chartPoint = chart.NSeries[0].Points[0];

            // Visa den aktuella YValueType.
            Console.WriteLine("Current YValueType: " + chartPoint.YValueType);

            // Visa YValue innan ändring
            Console.WriteLine("Current YValue: " + chartPoint.YValue);

            // Ändra YValue till en annan typ (string för att demonstrera typändring)
            chartPoint.YValue = "15"; // This will change the YValueType to IsString

            // Visa YValueType efter ändring
            Console.WriteLine("New YValueType: " + chartPoint.YValueType);
            Console.WriteLine("New YValue: " + chartPoint.YValue);

            // Spara arbetsboken
            workbook.Save("ChartPointPropertyYValueTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [CellValueType](../../../aspose.cells/cellvaluetype/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


