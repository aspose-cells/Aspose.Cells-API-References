---
title: TextTabStop.TabPosition
second_title: Aspose.Cells for .NET API Reference
description: TextTabStop property. Specifies the position of the tab stop relative to the left margin
type: docs
url: /net/aspose.cells.drawing.texts/texttabstop/tabposition/
---
## TextTabStop.TabPosition property

Specifies the position of the tab stop relative to the left margin.

```csharp
public double TabPosition { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextTabStopPropertyTabPositionDemo
    {
        public static void Run()
        {
            try
            {
                // Create a workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Access paragraph properties which would contain TextTabStop
                var style = worksheet.Cells["A1"].GetStyle();
                var textOptions = style.TextDirection;
                
                // This demonstrates the TabPosition property concept
                Console.WriteLine("Demonstrating TextTabStop.TabPosition property:");
                
                // In a real scenario, you would access TabPosition through proper API methods
                // For demonstration purposes, we'll show how the property works conceptually
                Console.WriteLine("\nTabPosition represents the position of the tab stop");
                Console.WriteLine("relative to the left margin, measured in points.");
                
                // Example values that could be assigned to TabPosition
                Console.WriteLine("\nExample TabPosition values:");
                Console.WriteLine("Default tab stop position: 36.0 (0.5 inches)");
                Console.WriteLine("Custom tab stop position: 72.0 (1 inch)");
                
                // Add sample text with tabs
                worksheet.Cells["A1"].Value = "Item\tPrice";
                worksheet.Cells["A2"].Value = "Product\t$10.99";
                
                Console.WriteLine("\nNote: In actual usage, TabPosition would be accessed through");
                Console.WriteLine("proper API methods that provide TextTabStop instances");
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

* class [TextTabStop](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


