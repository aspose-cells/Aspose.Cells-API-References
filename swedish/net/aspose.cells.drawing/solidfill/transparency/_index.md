---
title: "SolidFill.Transparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SolidFill-egenskap. Returnerar eller anger transparensgraden för området som ett värde från 0,0 (opak) till 1,0 (klar)"
type: docs
url: /sv/net/aspose.cells.drawing/solidfill/transparency/
---
## SolidFill.Transparency property

Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar).

```csharp
public double Transparency { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett exempeldiagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            // Lägg till en form för att demonstrera transparens
            Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.FreeFloating, 
                1000, 1000, 2000, 2000);
            
            // Ange solid fyllning med transparens
            shape.Fill.SolidFill.Color = Color.Blue;
            shape.Fill.SolidFill.Transparency = 0.5; // 50% transparent

            // Lägg till en annan form för jämförelse (helt opak)
            Shape shape2 = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.FreeFloating, 
                3000, 1000, 2000, 2000);
            shape2.Fill.SolidFill.Color = Color.Blue;
            shape2.Fill.SolidFill.Transparency = 0; // 0% transparent (fully opaque)

            // Spara arbetsboken
            workbook.Save("SolidFillTransparencyDemo.xlsx");
        }
    }
}
```

### Se även

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


