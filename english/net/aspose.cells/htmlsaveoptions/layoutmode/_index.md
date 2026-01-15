---
title: HtmlSaveOptions.LayoutMode
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Gets or sets the layout mode when saving to HTML. The default value is Normal
type: docs
url: /net/aspose.cells/htmlsaveoptions/layoutmode/
---
## HtmlSaveOptions.LayoutMode property

Gets or sets the layout mode when saving to HTML. The default value is Normal

```csharp
public HtmlLayoutMode LayoutMode { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyLayoutModeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Layout Mode Test");

            try
            {
                // Create HtmlSaveOptions instance
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Display the current LayoutMode value
                Console.WriteLine("Current LayoutMode: " + options.LayoutMode);

                // Set LayoutMode to Print
                options.LayoutMode = HtmlLayoutMode.Print;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Save the workbook with Print layout mode
                workbook.Save("LayoutModePrint.html", options);

                // Set LayoutMode to Normal
                options.LayoutMode = HtmlLayoutMode.Normal;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Save the workbook with Normal layout mode
                workbook.Save("LayoutModeNormal.html", options);

                Console.WriteLine("HTML files saved with different LayoutMode settings.");
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

* enum [HtmlLayoutMode](../../../aspose.cells.rendering/htmllayoutmode/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


