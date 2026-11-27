---
title: "Chart.ActualChartSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart-egenskap. Hämtar den faktiska storleken på diagrammet i pixelenheter"
type: docs
url: /sv/net/aspose.cells.charts/chart/actualchartsize/
---
## Chart.ActualChartSize property

Hämtar den faktiska storleken på diagrammet i pixelenheter.

```csharp
[Obsolete("Use Chart.GetActualSize() method instead.")]
public Size ActualChartSize { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället metoden Chart.GetActualSize(). Denna egenskap kommer att tas bort 12 månader senare från och med juli 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyActualChartSizeDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Beräkna diagrammet för att säkerställa att egenskaperna är fyllda
            chart.Calculate();

            // Demonstrera användning av ActualChartSize
            Console.WriteLine($"Actual Chart Size - Width: {chart.ActualChartSize.Width}, Height: {chart.ActualChartSize.Height}");

            // Lägg till en form vars storlek baseras på ActualChartSize
            Shape shape = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Rectangle,
                PlacementType.Move,
                0.5,  // x position (relative)
                0.5,  // y position (relative)
                0.5 + (0.1 * chart.ActualChartSize.Height / chart.ActualChartSize.Width),  // width adjusted by aspect ratio
                0.6   // height
            );
            shape.Fill.SolidFill.Color = Color.Blue;

            // Spara arbetsboken
            workbook.Save("ChartWithActualSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


