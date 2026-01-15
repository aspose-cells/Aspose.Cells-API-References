---
title: Range.ClearHyperlinks
second_title: Aspose.Cells for .NET API Reference
description: Range method. Only removes hyperlinks
type: docs
url: /net/aspose.cells/range/clearhyperlinks/
---
## Range.ClearHyperlinks method

Only removes hyperlinks.

```csharp
public void ClearHyperlinks(bool clearFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| clearFormat | Boolean | Indicates whether to clear the format of hyperlinks. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearHyperlinksWithBooleanDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a range and add some hyperlinks for demonstration
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");
            range.AddHyperlink("https://www.example.com", "Example", "Visit Example");

            try
            {
                // Clear hyperlinks with format preservation (false)
                range.ClearHyperlinks(false);
                Console.WriteLine("Hyperlinks cleared while preserving format");

                // Add hyperlinks again
                range.AddHyperlink("https://www.aspose.com", "Aspose", "Visit Aspose");

                // Clear hyperlinks without format preservation (true)
                range.ClearHyperlinks(true);
                Console.WriteLine("Hyperlinks cleared without preserving format");

                // Save the workbook
                workbook.Save("ClearHyperlinksDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
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

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


