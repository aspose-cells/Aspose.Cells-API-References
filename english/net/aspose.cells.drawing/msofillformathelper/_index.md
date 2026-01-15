---
title: Class MsoFillFormatHelper
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.MsoFillFormatHelper class. Represents fill formatting for a shape
type: docs
url: /net/aspose.cells.drawing/msofillformathelper/
---
## MsoFillFormatHelper class

Represents fill formatting for a shape.

```csharp
public class MsoFillFormatHelper
```

## Properties

| Name | Description |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformathelper/backcolor/) { get; set; } | Gets and sets the file back color. |
| [ForeColor](../../aspose.cells.drawing/msofillformathelper/forecolor/) { get; set; } | Gets and sets the fill fore color. |
| [ForeColorTransparency](../../aspose.cells.drawing/msofillformathelper/forecolortransparency/) { get; set; } | Returns or sets the degree of fore color of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
| [ImageData](../../aspose.cells.drawing/msofillformathelper/imagedata/) { get; set; } | Gets and sets the Texture and Picture fill data. |
| [IsVisible](../../aspose.cells.drawing/msofillformathelper/isvisible/) { get; set; } | Indicates whether there is fill. |
| [Texture](../../aspose.cells.drawing/msofillformathelper/texture/) { get; } | Gets the texture fill type. |

## Methods

| Name | Description |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformathelper/setonecolorgradient/)(Color, double, GradientStyleType, int) | Sets the specified fill to a one-color gradient. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;
    using System.Reflection;

    public class DrawingClassMsoFillFormatHelperDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "MsoFillFormatHelper Demo";

            try
            {
                // Create an instance of MsoFillFormatHelper using reflection
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Set basic properties
                fillHelper.ForeColor = Color.FromArgb(255, 100, 150, 200);
                fillHelper.ForeColorTransparency = 0.3;
                fillHelper.BackColor = Color.LightGray;
                fillHelper.IsVisible = true;

                // Display property values
                Console.WriteLine($"ForeColor: {fillHelper.ForeColor}");
                Console.WriteLine($"ForeColorTransparency: {fillHelper.ForeColorTransparency}");
                Console.WriteLine($"BackColor: {fillHelper.BackColor}");
                Console.WriteLine($"IsVisible: {fillHelper.IsVisible}");
                Console.WriteLine($"Texture (read-only): {fillHelper.Texture}");

                // Save the workbook
                workbook.Save("MsoFillFormatHelperDemo.xlsx");
                Console.WriteLine("MsoFillFormatHelper demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in MsoFillFormatHelper demo: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


