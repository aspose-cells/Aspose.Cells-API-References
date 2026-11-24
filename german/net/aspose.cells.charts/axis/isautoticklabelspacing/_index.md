---
title: "Axis.IsAutoTickLabelSpacing"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Axis-Eigenschaft. Gibt an, ob der Abstand der Tick-Beschriftungen automatisch ist"
type: docs
url: /de/net/aspose.cells.charts/axis/isautoticklabelspacing/
---
## Axis.IsAutoTickLabelSpacing property

Gibt an, ob der Abstand der Achsenbeschriftungen automatisch ist

```csharp
public bool IsAutoTickLabelSpacing { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutoTickLabelSpacingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Werteachse konfigurieren
            Axis valueAxis = chart.ValueAxis;
            valueAxis.IsAutoTickLabelSpacing = true; // Core property demonstration
            
            // Kategorienachse konfigurieren
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.IsAutoTickLabelSpacing = false; // Core property demonstration
            categoryAxis.TickLabelSpacing = 2;

            workbook.Save("AxisPropertyIsAutoTickLabelSpacingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


