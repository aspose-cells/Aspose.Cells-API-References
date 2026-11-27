---
title: "ChartPoint.DataLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Returnerar ett DataLabels-objekt som representerar datalabelen som är associerad med denna diagrampunkt"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/datalabels/
---
## ChartPoint.DataLabels property

Returnerar ett `DataLabels`-objekt som representerar datalabelen som är associerad med denna diagrampunkt.

```csharp
public DataLabels DataLabels { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyDataLabelsDemo
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

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Kom åt den första diagrampunkten
                ChartPoint point = chart.NSeries[0].Points[0];

                // Hämta DataLabels-egenskapen (skrivskyddad)
                DataLabels dataLabels = point.DataLabels;

                // Visa DataLabels-egenskaper
                Console.WriteLine("DataLabels ShowValue: " + dataLabels.ShowValue);
                Console.WriteLine("DataLabels ShowCategoryName: " + dataLabels.ShowCategoryName);
                Console.WriteLine("DataLabels ShowSeriesName: " + dataLabels.ShowSeriesName);
                Console.WriteLine("DataLabels Position: " + dataLabels.Position);

                // Ändra några DataLabels-egenskaper (eftersom DataLabels inte är skrivskyddad)
                dataLabels.ShowValue = true;
                dataLabels.ShowCategoryName = true;
                dataLabels.Position = LabelPositionType.OutsideEnd;

                // Spara resultatet
                workbook.Save("ChartPointDataLabelsDemo.xlsx");
                Console.WriteLine("DataLabels demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [DataLabels](../../datalabels/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


