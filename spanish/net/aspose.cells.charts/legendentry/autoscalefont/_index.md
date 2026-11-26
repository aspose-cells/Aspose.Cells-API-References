---
title: "LegendEntry.AutoScaleFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LegendEntry. Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. El valor predeterminado es Verdadero"
type: docs
url: /es/net/aspose.cells.charts/legendentry/autoscalefont/
---
## LegendEntry.AutoScaleFont property

True si el texto en el objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor predeterminado es True.

```csharp
public bool AutoScaleFont { get; set; }
```

### Ejemplos

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

### Ver también

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


