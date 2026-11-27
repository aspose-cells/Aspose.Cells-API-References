---
title: "FillFormat.GradientDegree"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Returnerar gradientgraden för den angivna fyllningen. Gäller endast för Excel 2007"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/gradientdegree/
---
## FillFormat.GradientDegree property

Returnerar gradientens grad för den angivna fyllningen. Gäller endast för Excel 2007.

```csharp
public double GradientDegree { get; }
```

### Anmärkningar

Kan endast vara ett värde från 0.0 (mörk) till 1.0 (ljus).

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientDegreeDemo
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

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ställ in gradientfyllning för den första serien
            Aspose.Cells.Drawing.FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;
            fillFormat.SetTwoColorGradient(Color.Red, Color.Blue, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 2);
            
            // Visa gradientgraden
            Console.WriteLine("Gradient Degree: " + fillFormat.GradientDegree);

            // Spara arbetsboken
            workbook.Save("GradientDegreeDemo.xlsx");
        }
    }
}
```

### Se även

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


