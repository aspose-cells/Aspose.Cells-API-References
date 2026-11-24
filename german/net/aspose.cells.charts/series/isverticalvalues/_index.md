---
title: "Series.IsVerticalValues"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series‑Eigenschaft. Gibt an, ob die Datenquelle vertikal ist"
type: docs
url: /de/net/aspose.cells.charts/series/isverticalvalues/
---
## Series.IsVerticalValues property

Gibt an, ob die Datenquelle vertikal ist.

```csharp
public bool IsVerticalValues { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsVerticalValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i-1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }

            // Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Serie mit vertikalen Werten hinzufügen
            chart.NSeries.Add("A1:B10", true);
            
            // Demonstration der IsVerticalValues‑Eigenschaft (schreibgeschützt)
            Console.WriteLine("IsVerticalValues for first series: " + chart.NSeries[0].IsVerticalValues);
            
            // Um die Ausrichtung zu ändern, müssen wir die Serie mit anderen Parametern neu erstellen
            chart.NSeries.Clear();
            chart.NSeries.Add("A1:B10", false);
            Console.WriteLine("IsVerticalValues after recreation: " + chart.NSeries[0].IsVerticalValues);
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


