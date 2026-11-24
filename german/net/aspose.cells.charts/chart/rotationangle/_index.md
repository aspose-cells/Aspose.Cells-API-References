---
title: "Chart.RotationAngle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Diagramm-Eigenschaft. Stellt die Drehung der 3D-Diagrammansicht dar, die Drehung des Plotbereichs um die Z-Achse in Grad"
type: docs
url: /de/net/aspose.cells.charts/chart/rotationangle/
---
## Chart.RotationAngle property

Stellt die Drehung der 3‑D‑Diagrammansicht dar (die Drehung des Zeichenbereichs um die Z‑Achse in Grad).

```csharp
public int RotationAngle { get; set; }
```

### Hinweise

Der Wert dieser Eigenschaft muss zwischen 0 und 360 liegen, außer bei 3‑D-Balkendiagrammen, wo der Wert zwischen 0 und 44 liegen muss. Der Standardwert ist 20. Gilt nur für 3‑D-Diagramme.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyRotationAngleDemo
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

            // Ein 3D‑Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setzen Sie den Rotationswinkel auf 45 Grad
            chart.RotationAngle = 45;

            // Speichere die Arbeitsmappe
            workbook.Save("ChartRotationAngleDemo.xlsx");

            Console.WriteLine("Chart with rotation angle created successfully.");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


