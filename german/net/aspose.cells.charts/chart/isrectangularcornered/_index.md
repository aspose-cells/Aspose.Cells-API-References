---
title: "Chart.IsRectangularCornered"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Diagramm-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob der Diagrammbereich rechteckig mit Ecken ist. Standard ist true."
type: docs
url: /de/net/aspose.cells.charts/chart/isrectangularcornered/
---
## Chart.IsRectangularCornered property

Liefert oder setzt einen Wert, der angibt, ob der Diagrammbereich rechteckige Ecken hat. Standard ist true.

```csharp
public bool IsRectangularCornered { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyIsRectangularCorneredDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demonstration der IsRectangularCornered-Eigenschaft
            Console.WriteLine("Default IsRectangularCornered: " + chart.IsRectangularCornered);
            
            // Auf true setzen, um die Diagrammecken rechteckig zu machen.
            chart.IsRectangularCornered = true;
            Console.WriteLine("After setting IsRectangularCornered to true: " + chart.IsRectangularCornered);

            // Speichere die Arbeitsmappe
            workbook.Save("ChartPropertyIsRectangularCorneredDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


