---
title: "ChartFrame.AutoScaleFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame property. True if texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är True"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/autoscalefont/
---
## ChartFrame.AutoScaleFont property

Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant.

```csharp
public virtual bool AutoScaleFont { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyAutoScaleFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till diagramrubriken
            chart.Title.Text = "Sample Chart";
            
            // Demonstrera egenskapen AutoScaleFont
            chart.Title.AutoScaleFont = true;
            Console.WriteLine("Chart title AutoScaleFont is set to: " + chart.Title.AutoScaleFont);

            // Spara arbetsboken
            workbook.Save("ChartFrameAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


