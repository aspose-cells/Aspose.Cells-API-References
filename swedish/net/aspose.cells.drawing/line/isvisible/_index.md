---
title: "Line.IsVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Line-egenskap. Anger om linjen är synlig"
type: docs
url: /sv/net/aspose.cells.drawing/line/isvisible/
---
## Line.IsVisible property

Anger om linjen är synlig.

```csharp
public bool IsVisible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LinePropertyIsVisibleDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Åtkomst till huvudrutnätlinjer och ange synlighet
            chart.CategoryAxis.MajorGridLines.IsVisible = true;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Verifiera synligheten
            Console.WriteLine("Major Gridlines Visible: " + chart.CategoryAxis.MajorGridLines.IsVisible);
        }
    }
}
```

### Se även

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


