---
title: "Axis.IsVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Achsen-Eigenschaft. Gibt an, ob die Achse sichtbar ist"
type: docs
url: /de/net/aspose.cells.charts/axis/isvisible/
---
## Axis.IsVisible property

Gibt an, ob die Achse sichtbar ist.

```csharp
public bool IsVisible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Füge eine sekundäre Achsenreihe hinzu
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries[1].PlotOnSecondAxis = true;

            // Demonstrieren Sie die IsVisible-Eigenschaft
            Console.WriteLine("Secondary Value Axis Visible: " + chart.SecondValueAxis.IsVisible);
            
            // Verstecke die sekundäre Achse
            chart.SecondValueAxis.IsVisible = false;
            Console.WriteLine("After setting to false - Secondary Value Axis Visible: " + chart.SecondValueAxis.IsVisible);

            // Speichere die Arbeitsmappe
            workbook.Save("AxisIsVisibleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


