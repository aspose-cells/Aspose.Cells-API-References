---
title: CustomRenderSettings.GetCellBorderWidth
second_title: Aspose.Cells for .NET API Reference
description: CustomRenderSettings method. Specifies cell border width according to border type
type: docs
url: /net/aspose.cells.rendering/customrendersettings/getcellborderwidth/
---
## CustomRenderSettings.GetCellBorderWidth method

Specifies cell border width according to border type.

```csharp
public virtual float GetCellBorderWidth(CellBorderType borderType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| borderType | CellBorderType | cell border type |

### Return Value

cell border width

### Remarks

Any negative value will be ignored.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodGetCellBorderWidthWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data for context
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Create an instance of CustomRenderSettings
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // Call GetCellBorderWidth with different border types
                float thinBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // Display the results
                Console.WriteLine($"Thin border width: {thinBorderWidth}");
                Console.WriteLine($"Thick border width: {thickBorderWidth}");
                Console.WriteLine($"Dashed border width: {dashedBorderWidth}");

                // Save the workbook
                workbook.Save("GetCellBorderWidthDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [CellBorderType](../../../aspose.cells/cellbordertype/)
* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


