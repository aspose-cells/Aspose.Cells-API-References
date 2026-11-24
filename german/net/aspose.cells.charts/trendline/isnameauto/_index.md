---
title: "Trendline.IsNameAuto"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Trendline‑Eigenschaft. Gibt zurück, ob Microsoft Excel den Namen der Trendlinie automatisch bestimmt"
type: docs
url: /de/net/aspose.cells.charts/trendline/isnameauto/
---
## Trendline.IsNameAuto property

Gibt zurück, ob Microsoft Excel den Namen der Trendlinie automatisch bestimmt.

```csharp
public bool IsNameAuto { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyIsNameAutoDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Serie zum Diagramm hinzufügen
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Trendlinie hinzufügen – modifiziert, um die korrekte Erstellung des Trendlinienobjekts sicherzustellen
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // IsNameAuto‑Eigenschaft demonstrieren
            Console.WriteLine("Initial IsNameAuto value: " + trendline.IsNameAuto);
            
            // Benutzerdefinierten Namen festlegen (deaktiviert automatische Namensgebung)
            trendline.Name = "Custom Trendline Name";
            Console.WriteLine("After setting custom name, IsNameAuto: " + trendline.IsNameAuto);
            
            // Zur automatischen Namensgebung zurücksetzen
            trendline.IsNameAuto = true;
            Console.WriteLine("After setting IsNameAuto=true, Name: " + trendline.Name);
        }
    }
}
```

### Siehe auch

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


