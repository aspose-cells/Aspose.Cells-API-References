---
title: "ChartShape.Chart"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartShape-Eigenschaft. Gibt ein Chart-Objekt zurück, das das im Objekt enthaltene Diagramm darstellt"
type: docs
url: /de/net/aspose.cells.drawing/chartshape/chart/
---
## ChartShape.Chart property

Gibt ein Chart-Objekt zurück, das das im Objekt enthaltene Diagramm darstellt.

```csharp
public Chart Chart { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartShapePropertyChartDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Rufen Sie die ChartShape-Instanz ab
            ChartShape chartShape = (ChartShape)chart.ChartObject;

            // Greifen Sie auf die Chart-Eigenschaft zu (schreibgeschützt)
            Chart accessedChart = chartShape.Chart;

            // Diagrammeigenschaften anzeigen
            Console.WriteLine("Chart Name: " + accessedChart.Name);
            Console.WriteLine("Chart Type: " + accessedChart.Type);
            Console.WriteLine("Show Legend: " + accessedChart.ShowLegend);

            // Diagrammeigenschaften über das Chart-Objekt ändern
            accessedChart.Name = "Sales Chart";
            accessedChart.ShowLegend = false;
            accessedChart.Title.Text = "Product Sales Distribution";

            // Diagrammtyp ändern
            accessedChart.Type = ChartType.Pie;

            // Ergebnis speichern
            workbook.Save("ChartShapePropertyChartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../../../aspose.cells.charts/chart/)
* class [ChartShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


