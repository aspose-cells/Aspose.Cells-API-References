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
namespace AsposeCellsExamples
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

            // Create a union range covering cells A1 to B2
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            // Add some data for context
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "More Data";

            try
            {
                // Create a style with specific formatting
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.Font.Color = Color.Red;
                style.ForegroundColor = Color.LightBlue;
                style.Pattern = BackgroundType.Solid;
                style.HorizontalAlignment = TextAlignmentType.Center;

                // Create a StyleFlag to specify which properties to apply
                StyleFlag flag = new StyleFlag();
                flag.FontBold = true;
                flag.FontColor = true;
                flag.CellShading = true;
                flag.HorizontalAlignment = true;

                // Call ApplyStyle with the style and flag parameters
                unionRange.ApplyStyle(style, flag);

                Console.WriteLine("ApplyStyle method called successfully");
                Console.WriteLine($"Applied style to range: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ApplyStyle: {ex.Message}");
            }

            // Save the workbook
            workbook.Save("UnionRangeMethodApplyStyleWithStyleStyleFlagDemo.xlsx");
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


