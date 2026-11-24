---
title: "LegendEntry.AutoScaleFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LegendEntry-Eigenschaft. True, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße sich ändert. Der Standardwert ist True"
type: docs
url: /de/net/aspose.cells.charts/legendentry/autoscalefont/
---
## LegendEntry.AutoScaleFont property

True, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße geändert wird. Der Standardwert ist True.

```csharp
public bool AutoScaleFont { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyAutoScaleFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("Widget A");
            sheet.Cells["A3"].PutValue("Widget B");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1500);
            sheet.Cells["B3"].PutValue(3000);

            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 15, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            LegendEntry firstEntry = chart.Legend.LegendEntries[0];
            firstEntry.AutoScaleFont = true;
            firstEntry.Font.Size = 14;

            workbook.Save("LegendEntryAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


