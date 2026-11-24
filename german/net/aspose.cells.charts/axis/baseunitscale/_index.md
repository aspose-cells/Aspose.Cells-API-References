---
title: "Axis.BaseUnitScale"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Achsen‑Eigenschaft. Stellt die Basiseinheitsskala für die Kategorienachse dar"
type: docs
url: /de/net/aspose.cells.charts/axis/baseunitscale/
---
## Axis.BaseUnitScale property

Stellt die Basiseinheitsskala für die Kategorienachse dar.

```csharp
public TimeUnit BaseUnitScale { get; set; }
```

### Hinweise

Wirkt nur, wenn die CategoryType‑Eigenschaft auf TimeScale gesetzt ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyBaseUnitScaleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddDays(i));
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Basiseinheitsskala für die Kategorienachse festlegen
            chart.CategoryAxis.BaseUnitScale = TimeUnit.Months;

            // Speichere die Arbeitsmappe
            workbook.Save("AxisPropertyBaseUnitScaleDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


