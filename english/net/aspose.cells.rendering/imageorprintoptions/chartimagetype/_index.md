---
title: ImageOrPrintOptions.ChartImageType
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Indicate the chart imagetype when converting. default value PNG
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/chartimagetype/
---
## ImageOrPrintOptions.ChartImageType property

Indicate the chart imagetype when converting. default value: PNG.

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ChartImageType { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples.ImageOrPrintOptionsPropertyChartImageTypeDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Charts;
    using System;

    public class ImageOrPrintOptionsPropertyChartImageTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook and populate data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(35);
            worksheet.Cells["B3"].PutValue(20);

            // Create a column chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Initialize ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Display current image format (default PNG)
            Console.WriteLine("Initial ImageType: " + options.ImageType);

            // Render chart as JPEG
            options.ImageType = ImageType.Jpeg;
            chart.ToImage("chart_output.jpg", options);
            Console.WriteLine("Generated JPEG image with ImageType: " + options.ImageType);

            // Render chart as PNG
            options.ImageType = ImageType.Png;
            chart.ToImage("chart_output.png", options);
            Console.WriteLine("Generated PNG image with ImageType: " + options.ImageType);
        }
    }
}
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


