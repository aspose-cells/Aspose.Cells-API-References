---
title: "Chart.SizeWithWindow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart egenskap. Sant om Microsoft Excel ändrar storlek på diagrammet för att matcha storleken på diagrambladets fönster"
type: docs
url: /sv/net/aspose.cells.charts/chart/sizewithwindow/
---
## Chart.SizeWithWindow property

Sant om Microsoft Excel ändrar diagrammets storlek så att den matchar storleken på diagrambladets fönster.

```csharp
public bool SizeWithWindow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySizeWithWindowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
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
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Demonstrera SizeWithWindow egenskap
            Console.WriteLine("Default SizeWithWindow: " + chart.SizeWithWindow);
            
            // Aktivera SizeWithWindow
            chart.SizeWithWindow = true;
            Console.WriteLine("After setting SizeWithWindow to true: " + chart.SizeWithWindow);
            
            // Spara arbetsboken
            workbook.Save("ChartSizeWithWindowDemo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


