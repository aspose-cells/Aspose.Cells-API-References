---
title: "Chart.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Gibt den Namen des Diagramms zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.charts/chart/name/
---
## Chart.Name property

Liest und setzt den Namen des Diagramms.

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Diagrammnamen anzeigen
            Console.WriteLine("Chart Name: " + chart.Name);

            // Ein weiteres Diagramm hinzufügen und dessen Namen anzeigen
            int chartIndex2 = worksheet.Charts.Add(ChartType.Pie, 20, 0, 30, 5);
            Aspose.Cells.Charts.Chart chart2 = worksheet.Charts[chartIndex2];
            chart2.NSeries.Add("B2:B4", true);
            chart2.NSeries.CategoryData = "A2:A4";
            Console.WriteLine("Second Chart Name: " + chart2.Name);
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


