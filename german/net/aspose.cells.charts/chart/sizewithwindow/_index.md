---
title: "Chart.SizeWithWindow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Wahr, wenn Microsoft Excel das Diagramm an die Größe des Diagrammblattfensters anpasst"
type: docs
url: /de/net/aspose.cells.charts/chart/sizewithwindow/
---
## Chart.SizeWithWindow property

True, wenn Microsoft Excel das Diagramm an die Größe des Diagrammblatt‑Fensters anpasst.

```csharp
public bool SizeWithWindow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySizeWithWindowDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // SizeWithWindow‑Eigenschaft demonstrieren
            Console.WriteLine("Default SizeWithWindow: " + chart.SizeWithWindow);
            
            // SizeWithWindow aktivieren
            chart.SizeWithWindow = true;
            Console.WriteLine("After setting SizeWithWindow to true: " + chart.SizeWithWindow);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ChartSizeWithWindowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


