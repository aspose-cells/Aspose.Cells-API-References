---
title: MsoFillFormatHelper.ForeColorTransparency
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormatHelper property. Returns or sets the degree of fore color of the specified fill as a value from 0.0 opaque through 1.0 clear
type: docs
url: /net/aspose.cells.drawing/msofillformathelper/forecolortransparency/
---
## MsoFillFormatHelper.ForeColorTransparency property

Returns or sets the degree of fore color of the specified fill as a value from 0.0 (opaque) through 1.0 (clear).

```csharp
public double ForeColorTransparency { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyForeColorTransparencyDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a label to make the example meaningful
            worksheet.Cells["A1"].Value = "ForeColorTransparency Demo";

            try
            {
                // Create an instance of MsoFillFormatHelper using reflection (no public constructor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Display the default ForeColorTransparency value
                Console.WriteLine($"Default ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // Set a new ForeColor and ForeColorTransparency
                fillHelper.ForeColor = Color.Blue;
                fillHelper.ForeColorTransparency = 0.5; // 50% transparency

                // Display the updated values
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");
                Console.WriteLine($"Updated ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // Demonstrate reading the transparency value
                double transparency = fillHelper.ForeColorTransparency;
                Console.WriteLine($"Current transparency level: {transparency} (0.0=opaque, 1.0=clear)");

                // Save the workbook to demonstrate successful execution
                workbook.Save("ForeColorTransparencyDemo.xlsx");

                Console.WriteLine("ForeColorTransparency property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColorTransparency demo: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


