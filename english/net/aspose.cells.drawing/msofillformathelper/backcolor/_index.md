---
title: MsoFillFormatHelper.BackColor
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormatHelper property. Gets and sets the file back color
type: docs
url: /net/aspose.cells.drawing/msofillformathelper/backcolor/
---
## MsoFillFormatHelper.BackColor property

Gets and sets the file back color.

```csharp
public Color BackColor { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyBackColorDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a label just to have some content in the sheet
            worksheet.Cells["A1"].Value = "BackColor Property Demo";

            try
            {
                // MsoFillFormatHelper does not expose a public constructor, use reflection to instantiate it
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Set the BackColor to a known color (e.g., LightCoral)
                fillHelper.BackColor = Color.LightCoral;

                // Read back the BackColor value and display it
                Console.WriteLine($"BackColor is set to: {fillHelper.BackColor}");

                // Optionally you could also read the ForeColor to show it remains default
                Console.WriteLine($"ForeColor (default) : {fillHelper.ForeColor}");

                // Save the workbook – the fill helper is not attached to a shape,
                // but saving demonstrates that the code ran without error.
                workbook.Save("BackColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during BackColor demo: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


