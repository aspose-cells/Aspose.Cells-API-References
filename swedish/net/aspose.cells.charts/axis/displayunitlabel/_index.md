---
title: "Axis.DisplayUnitLabel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Representerar en enhetsetikett på en axel i det angivna diagrammet. Enhetsetiketter är användbara för att diagrammera stora värden, till exempel i miljoner eller miljarder"
type: docs
url: /sv/net/aspose.cells.charts/axis/displayunitlabel/
---
## Axis.DisplayUnitLabel property

Representerar en enhetsetikett på en axel i det angivna diagrammet. Enhetsetiketter är användbara för att diagrammera stora värden – till exempel i miljoner eller miljarder.

```csharp
public DisplayUnitLabel DisplayUnitLabel { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyDisplayUnitLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // Skapa diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("A1:A4", true);
            
            // Konfigurera visningsenhet och etikett
            chart.ValueAxis.DisplayUnit = Aspose.Cells.Charts.DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Skriv ut texten för visningsenhetsetiketten
            Console.WriteLine("Display Unit Label: " + chart.ValueAxis.DisplayUnitLabel.Text);
            
            // Spara arbetsboken
            workbook.Save("AxisPropertyDisplayUnitLabelDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [DisplayUnitLabel](../../displayunitlabel/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


