---
title: Class CustomRenderSettings
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Rendering.CustomRenderSettings class. Represents custom settings during rendering
type: docs
url: /net/aspose.cells.rendering/customrendersettings/
---
## CustomRenderSettings class

Represents custom settings during rendering.

```csharp
public class CustomRenderSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [CustomRenderSettings](customrendersettings/)() | Ctor. |

## Methods

| Name | Description |
| --- | --- |
| virtual [GetCellBorderWidth](../../aspose.cells.rendering/customrendersettings/getcellborderwidth/)(CellBorderType) | Specifies cell border width according to border type. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "Border Width Test";

            try
            {
                // Create an instance of CustomRenderSettings using the default constructor
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Demonstrate the GetCellBorderWidth method with different border types
                float thinWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Display the results
                Console.WriteLine($"Thin border width: {thinWidth}");
                Console.WriteLine($"Thick border width: {thickWidth}");
                Console.WriteLine($"Dashed border width: {dashedWidth}");

                // Save the workbook
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("CustomRenderSettings demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CustomRenderSettings demonstration: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


