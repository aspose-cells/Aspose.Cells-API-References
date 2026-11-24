---
title: "Axis.MinorUnitScale"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Axis-Eigenschaft. Stellt die Haupt-Einheitsskala für die Kategorienachse dar"
type: docs
url: /de/net/aspose.cells.charts/axis/minorunitscale/
---
## Axis.MinorUnitScale property

Gibt die Skalierung der Haupteinheit für die Kategorienachse an.

```csharp
public TimeUnit MinorUnitScale { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinorUnitScaleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit Zeitbezug hinzufügen
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddMonths(i - 2));
                worksheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Kategorieachse als Zeitskala konfigurieren
            chart.CategoryAxis.CategoryType = CategoryType.TimeScale;
            chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
            chart.CategoryAxis.MinorUnit = 2;

            // Speichere die Arbeitsmappe
            workbook.Save("AxisPropertyMinorUnitScaleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


