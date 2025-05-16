---
title: UnionRange.SetStyle
second_title: Aspose.Cells for .NET API Reference
description: UnionRange method. Sets the style of the range
type: docs
url: /net/aspose.cells/unionrange/setstyle/
---
## UnionRange.SetStyle method

Sets the style of the range.

```csharp
public void SetStyle(Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The Style object. |

### Examples

```csharp
namespace AsposeCellsExamples.UnionRangeMethodSetStyleDemo
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetStyleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create sample data in cells
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Create a range (changed from CreateUnionRange to CreateRange)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Create a custom style
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;

            try
            {
                // Apply the style to the range
                range.SetStyle(style);

                Console.WriteLine("SetStyle method executed successfully with parameters (Style)");
                Console.WriteLine($"Style applied to range: {range.RefersTo}");
                
                // Display range information
                Console.WriteLine($"\nRange Info - FirstRow: {range.FirstRow}, FirstColumn: {range.FirstColumn}");
                Console.WriteLine($"RowCount: {range.RowCount}, ColumnCount: {range.ColumnCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStyle method: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("UnionRangeSetStyleDemo.xlsx");
        }
    }
}
```

### See Also

* class [Style](../../style/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


