---
title: MsoFillFormatHelper.IsVisible
second_title: Aspose.Cells for .NET API Reference
description: MsoFillFormatHelper property. Indicates whether there is fill
type: docs
url: /net/aspose.cells.drawing/msofillformathelper/isvisible/
---
## MsoFillFormatHelper.IsVisible property

Indicates whether there is fill.

```csharp
public bool IsVisible { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a label to make the example meaningful
            worksheet.Cells["A1"].Value = "IsVisible Property Demo";

            try
            {
                // Create an instance of MsoFillFormatHelper using reflection (no public constructor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Display the default IsVisible value
                Console.WriteLine($"Default IsVisible: {fillHelper.IsVisible}");

                // Set IsVisible to true
                fillHelper.IsVisible = true;
                Console.WriteLine($"After setting to true: {fillHelper.IsVisible}");

                // Set IsVisible to false
                fillHelper.IsVisible = false;
                Console.WriteLine($"After setting to false: {fillHelper.IsVisible}");

                // Read the current IsVisible value
                bool isVisible = fillHelper.IsVisible;
                Console.WriteLine($"Current IsVisible value: {isVisible}");

                // Save the workbook to demonstrate successful execution
                workbook.Save("IsVisibleDemo.xlsx");

                Console.WriteLine("IsVisible property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during IsVisible demo: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


