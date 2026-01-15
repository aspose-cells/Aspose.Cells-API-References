---
title: FillFormat.GradientFill
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Gets GradientFill object
type: docs
url: /net/aspose.cells.drawing/fillformat/gradientfill/
---
## FillFormat.GradientFill property

Gets `GradientFill` object.

```csharp
public GradientFill GradientFill { get; }
```

### Examples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientFillDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Provide some data for a chart
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Add a column chart
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Access the fill format of the first series area
                FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;

                // Apply a two‑color gradient to the series
                fillFormat.SetTwoColorGradient(Color.Red, Color.Blue,
                                               GradientStyleType.Horizontal, 2);

                // Retrieve the GradientFill object (read‑only property)
                GradientFill gradientFill = fillFormat.GradientFill;

                // Display some information about the gradient fill
                Console.WriteLine("GradientFill details:");
                Console.WriteLine($"  FillType      : {gradientFill.FillType}");
                Console.WriteLine($"  DirectionType: {gradientFill.DirectionType}");
                Console.WriteLine($"  Angle         : {gradientFill.Angle}");

                // Optionally modify the gradient angle using the set accessor
                gradientFill.Angle = 45.0f;
                Console.WriteLine($"  New Angle set to: {gradientFill.Angle}");

                // Save the workbook
                workbook.Save("FillFormatGradientFillDemo.xlsx");
                Console.WriteLine("Workbook saved as FillFormatGradientFillDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [GradientFill](../../gradientfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


