---
title: "FillFormat.GradientColor1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Returnerar gradientfärg 1 för den angivna fyllningen"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/gradientcolor1/
---
## FillFormat.GradientColor1 property

Returnerar gradientfärg 1 för den angivna fyllningen.

```csharp
public Color GradientColor1 { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientColor1Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Hämta fyllningsformat för den första serien
            FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;
            
            // Skapa gradientfyllning med korrekta parametertyper
            fillFormat.SetTwoColorGradient(
                Color.Red, 
                Color.White, 
                GradientStyleType.Horizontal, 
                1); // Gradient variant must be integer (1-4)

            // Hämta och visa gradientfärg
            Color gradientColor1 = fillFormat.GradientColor1;
            Console.WriteLine("Gradient Color 1: " + gradientColor1);
            Console.WriteLine("Gradient Degree: " + fillFormat.GradientDegree);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


