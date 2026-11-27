---
title: "DisplayUnitLabel.Text"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DisplayUnitLabel‑egenskap. Hämtar eller anger texten för displayenhetsetiketten"
type: docs
url: /sv/net/aspose.cells.charts/displayunitlabel/text/
---
## DisplayUnitLabel.Text property

Hämtar eller anger texten för displayenhetsetiketten.

```csharp
public override string Text { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DisplayUnitLabelPropertyTextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("A1:A4", true);
            
            // Konfigurera displayenhetsetiketten
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Kom åt och ändra texten för displayenhetsetiketten
            DisplayUnitLabel label = chart.ValueAxis.DisplayUnitLabel;
            Console.WriteLine("Default Display Unit Label: " + label.Text);
            
            // Ändra texten
            label.Text = "K Units";
            Console.WriteLine("Modified Display Unit Label: " + label.Text);
            
            // Spara arbetsboken
            workbook.Save("DisplayUnitLabelDemo.xlsx");
        }
    }
}
```

### Se även

* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


