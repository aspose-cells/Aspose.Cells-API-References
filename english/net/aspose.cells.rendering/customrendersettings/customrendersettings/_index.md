---
title: CustomRenderSettings.CustomRenderSettings
second_title: Aspose.Cells for .NET API Reference
description: CustomRenderSettings constructor. Ctor
type: docs
url: /net/aspose.cells.rendering/customrendersettings/customrendersettings/
---
## CustomRenderSettings constructor

Ctor.

```csharp
public CustomRenderSettings()
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data for context
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";

            try
            {
                // Create an instance of CustomRenderSettings using the constructor
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Display confirmation of successful constructor call
                Console.WriteLine("CustomRenderSettings instance created successfully using #ctor");

                // Demonstrate that the instance is functional by calling a method
                float borderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                Console.WriteLine($"Default thin border width: {borderWidth}");

                // Save the workbook
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomRenderSettings: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


