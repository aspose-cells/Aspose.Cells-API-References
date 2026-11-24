---
title: "Trendline.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Trendline-Eigenschaft. Gibt den Typ der Trendlinie zurück."
type: docs
url: /de/net/aspose.cells.charts/trendline/type/
---
## Trendline.Type property

Gibt den Trendlinientyp zurück.

```csharp
public TrendlineType Type { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["A5"].PutValue(4);
            
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(2);
            sheet.Cells["B3"].PutValue(4);
            sheet.Cells["B4"].PutValue(8);
            sheet.Cells["B5"].PutValue(16);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Serie hinzufügen
            chart.NSeries.Add("A2:A5", true);
            chart.NSeries[0].XValues = "B2:B5";

            // Exponentialtrendlinie hinzufügen.
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Demonstriere die Verwendung der Type‑Eigenschaft
            Console.WriteLine("Trendline type: " + trendline.Type);
            
            // Speichere die Arbeitsmappe
            workbook.Save("TrendlinePropertyTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TrendlineType](../../trendlinetype/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


