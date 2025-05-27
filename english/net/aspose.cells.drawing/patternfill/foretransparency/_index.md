---
title: PatternFill.ForeTransparency
second_title: Aspose.Cells for .NET API Reference
description: PatternFill property. Gets or sets the transparency of foreground color
type: docs
url: /net/aspose.cells.drawing/patternfill/foretransparency/
---
## PatternFill.ForeTransparency property

Gets or sets the transparency of foreground color.

```csharp
public double ForeTransparency { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForeTransparencyDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Access cell A1 and set sample text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with transparent pattern foreground");

            // Get cell style and configure pattern fill
            Style style = cell.GetStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.FromArgb(255, 0, 0); // Solid red (opaque)

            // Display initial transparency (0)
            double initialTransparency = (255 - style.ForegroundColor.A) / 255.0;
            Console.WriteLine("Initial ForeTransparency: " + initialTransparency);

            // Set new transparency (0=opaque, 1=fully transparent) by adjusting alpha
            double newTransparency = 0.6;
            int newAlpha = (int)((1 - newTransparency) * 255);
            style.ForegroundColor = Color.FromArgb(newAlpha, style.ForegroundColor.R, style.ForegroundColor.G, style.ForegroundColor.B);

            // Apply modified style to cell
            cell.SetStyle(style);

            // Create comparison cell with different transparency
            Cell cell2 = worksheet.Cells["B1"];
            cell2.PutValue("Comparison cell with 20% transparency");
            Style style2 = cell2.GetStyle();
            style2.Pattern = BackgroundType.Solid;
            style2.ForegroundColor = Color.FromArgb(0, 0, 255); // Solid blue (opaque)

            // Set 20% transparency
            double newTransparency2 = 0.2;
            int newAlpha2 = (int)((1 - newTransparency2) * 255);
            style2.ForegroundColor = Color.FromArgb(newAlpha2, style2.ForegroundColor.R, style2.ForegroundColor.G, style2.ForegroundColor.B);

            cell2.SetStyle(style2);

            // Auto-fit columns for better visibility
            worksheet.AutoFitColumn(0);
            worksheet.AutoFitColumn(1);

            // Save the modified workbook
            workbook.Save("ForeTransparencyDemo.xlsx");
        }
    }
}
```

### See Also

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


