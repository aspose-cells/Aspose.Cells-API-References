---
title: "Chart.ShowLegend"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Gibt einen Wert zurück oder setzt ihn, der angibt, ob die Diagrammlegende angezeigt wird. Standard ist true."
type: docs
url: /de/net/aspose.cells.charts/chart/showlegend/
---
## Chart.ShowLegend property

Liest oder setzt einen Wert, der angibt, ob die Diagrammlegende angezeigt wird. Standard ist true.

```csharp
public bool ShowLegend { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyShowLegendDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Legende standardmäßig anzeigen (true).
            Console.WriteLine("Legend initially visible: " + chart.ShowLegend);
            
            // Legende ausblenden.
            chart.ShowLegend = false;
            Console.WriteLine("Legend after setting to false: " + chart.ShowLegend);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartLegendExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


