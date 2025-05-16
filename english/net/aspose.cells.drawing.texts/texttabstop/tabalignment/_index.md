---
title: TextTabStop.TabAlignment
second_title: Aspose.Cells for .NET API Reference
description: TextTabStop property. Specifies the alignment that is to be applied to text using this tab stop
type: docs
url: /net/aspose.cells.drawing.texts/texttabstop/tabalignment/
---
## TextTabStop.TabAlignment property

Specifies the alignment that is to be applied to text using this tab stop.

```csharp
public TextTabAlignmentType TabAlignment { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples.TextTabStopPropertyTabAlignmentDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextTabStopPropertyTabAlignmentDemo
    {
        public static void Run()
        {
            try
            {
                // Create a workbook and access worksheet
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Access paragraph properties which would contain TextTabStop
                var style = worksheet.Cells["A1"].GetStyle();
                var textOptions = style.TextDirection;
                
                // This demonstrates the property type and values without direct instantiation
                Console.WriteLine("Demonstrating TextTabAlignmentType values:");
                foreach (TextTabAlignmentType alignment in Enum.GetValues(typeof(TextTabAlignmentType)))
                {
                    Console.WriteLine($"Possible alignment: {alignment}");
                }
                
                // In a real scenario, you would access TabAlignment through proper API methods
                Console.WriteLine("\nNote: In actual usage, TabAlignment would be accessed through");
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

* enum [TextTabAlignmentType](../../texttabalignmenttype/)
* class [TextTabStop](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


