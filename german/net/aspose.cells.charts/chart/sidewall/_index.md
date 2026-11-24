---
title: "Chart.SideWall"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart‑Eigenschaft. Gibt ein Walls‑Objekt zurück, das die Seitenwand eines 3D‑Diagramms darstellt."
type: docs
url: /de/net/aspose.cells.charts/chart/sidewall/
---
## Chart.SideWall property

Gibt ein [`Walls`](../walls/)‑Objekt zurück, das die Seitenwand eines 3‑D‑Diagramms darstellt.

```csharp
public Walls SideWall { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertySideWallDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // Ein 3D‑Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.SetChartDataRange("A1:C4", true);

            // Greifen Sie auf die SideWall‑Eigenschaft zu
            Walls sideWall = chart.SideWall;
            
            // Zeigen Sie einige Eigenschaften der SideWall an
            Console.WriteLine("SideWall properties:");
            Console.WriteLine("Width: " + sideWall.Width);
            Console.WriteLine("Height: " + sideWall.Height);
            Console.WriteLine("Depth: " + sideWall.Depth);

            // Berechnen Sie das Diagramm, um die Wandmaße zu aktualisieren
            chart.Calculate();

            // Aktualisierte Eigenschaften nach der Berechnung anzeigen
            Console.WriteLine("\nAfter Calculate():");
            Console.WriteLine("SideWall CenterX: " + sideWall.CenterX);
            Console.WriteLine("SideWall CenterY: " + sideWall.CenterY);
            Console.WriteLine("SideWall WidthPx: " + sideWall.WidthPx);
            Console.WriteLine("SideWall HeightPx: " + sideWall.HeightPx);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPropertySideWallDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


