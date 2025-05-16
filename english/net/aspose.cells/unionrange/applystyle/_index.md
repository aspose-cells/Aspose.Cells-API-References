---
title: UnionRange.ApplyStyle
second_title: Aspose.Cells for .NET API Reference
description: UnionRange method. Applies formats for a whole range
type: docs
url: /net/aspose.cells/unionrange/applystyle/
---
## UnionRange.ApplyStyle method

Applies formats for a whole range.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Remarks

Each cell in this range will contains a [`Style`](../../style/) object. So this is a memory-consuming method. Please use it carefully.

### Examples

```csharp
namespace AsposeCellsExamples.UnionRangeMethodApplyStyleWithStyleStyleFlagDemo
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create sample data in cells
            worksheet.Cells["A1"].PutValue("Header 1");
            worksheet.Cells["B1"].PutValue("Header 2");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Data 2");
            worksheet.Cells["B3"].PutValue(200);

            // Create a range
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Create a custom style
            Style style = workbook.CreateStyle();
            style.Font.Name = "Calibri";
            style.Font.Size = 11;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.LightYellow;
            style.Pattern = BackgroundType.Solid;
            style.HorizontalAlignment = TextAlignmentType.Center;

            // Create style flag to specify which properties to apply
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Font = true;
            styleFlag.CellShading = true;
            styleFlag.HorizontalAlignment = true;

            try
            {
                // Apply the style with specific flags to the range
                range.ApplyStyle(style, styleFlag);

                Console.WriteLine("ApplyStyle method executed successfully with parameters (Style, StyleFlag)");
                Console.WriteLine($"Style applied to range: {range.RefersTo}");

                // Display range information
                Console.WriteLine($"\nRange Info - FirstRow: {range.FirstRow}, FirstColumn: {range.FirstColumn}");
                Console.WriteLine($"RowCount: {range.RowCount}, ColumnCount: {range.ColumnCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ApplyStyle method: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("UnionRangeApplyStyleDemo.xlsx");
        }
    }
}
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


