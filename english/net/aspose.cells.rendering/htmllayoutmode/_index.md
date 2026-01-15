---
title: Enum HtmlLayoutMode
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Rendering.HtmlLayoutMode enum. Represents the layout mode for HTML rendering
type: docs
url: /net/aspose.cells.rendering/htmllayoutmode/
---
## HtmlLayoutMode enumeration

Represents the layout mode for HTML rendering.

```csharp
public enum HtmlLayoutMode
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Normal | `0` | Renders content like MS Excel. |
| Print | `1` | Renders content in print layout mode. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassHtmlLayoutModeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add some sample data to the worksheet
                worksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");
                worksheet.Cells["A2"].PutValue("This demonstrates HtmlLayoutMode");

                // Create HtmlSaveOptions and set layout mode to Normal
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                saveOptions.LayoutMode = HtmlLayoutMode.Normal;

                // Save the workbook with normal layout mode
                workbook.Save("NormalLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Normal layout mode.");

                // Change layout mode to Print
                saveOptions.LayoutMode = HtmlLayoutMode.Print;

                // Save the workbook with print layout mode
                workbook.Save("PrintLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Print layout mode.");

                // Display the enum values
                Console.WriteLine($"Normal mode value: {HtmlLayoutMode.Normal}");
                Console.WriteLine($"Print mode value: {HtmlLayoutMode.Print}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HtmlLayoutMode: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


