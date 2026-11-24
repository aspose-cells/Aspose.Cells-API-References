---
title: "Axis.LogBase"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Achsen‑Eigenschaft. Stellt die logarithmische Basis dar. Standardwert ist 10"
type: docs
url: /de/net/aspose.cells.charts/axis/logbase/
---
## Axis.LogBase property

Gibt die logarithmische Basis an. Der Standardwert ist 10.

```csharp
public double LogBase { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyLogBaseDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(Math.Pow(2, i-2)); // Exponential values
                worksheet.Cells[$"B{i}"].PutValue(i * 10);
            }

            // Ein Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Serie hinzufügen
            chart.NSeries.Add($"B2:B10", true);
            chart.NSeries[0].XValues = $"A2:A10";
            chart.NSeries[0].Name = "Logarithmic Series";

            // Logarithmische Achse konfigurieren
            chart.CategoryAxis.IsLogarithmic = true;
            chart.CategoryAxis.LogBase = 2; // Set logarithmic base to 2
            chart.CategoryAxis.Title.Text = "Logarithmic Scale (Base 2)";
            
            // Speichere die Arbeitsmappe
            workbook.Save("AxisPropertyLogBaseDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


