---
title: Style.IsModified
second_title: Aspose.Cells for .NET API Reference
description: Style method. Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell
type: docs
url: /net/aspose.cells/style/ismodified/
---
## Style.IsModified method

Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell.

```csharp
public bool IsModified(StyleModifyFlag modifyFlag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| modifyFlag | StyleModifyFlag | Style modified flags |

### Return Value

true if the specified properties have been modified

### Examples

```csharp
// Called: bool isHorizontalAlignmentModified = style.IsModified(StyleModifyFlag.HorizontalAlignment);
public static void Method_StyleModifyFlag_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Set some values in the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Sample Text&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(123.45);

            // Create a new style
            Style style = workbook.CreateStyle();
            style.Font.Name = &quot;Arial&quot;;
            style.Font.Size = 12;
            style.Font.Color = System.Drawing.Color.Blue;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;

            // Apply the style to a cell
            worksheet.Cells[&quot;A1&quot;].SetStyle(style);

            // Check which style properties have been modified
            bool isFontModified = style.IsModified(StyleModifyFlag.Font);
            bool isFontSizeModified = style.IsModified(StyleModifyFlag.FontSize);
            bool isFontColorModified = style.IsModified(StyleModifyFlag.FontColor);
            bool isHorizontalAlignmentModified = style.IsModified(StyleModifyFlag.HorizontalAlignment);

            // Output the results
            Console.WriteLine(&quot;Font Modified: &quot; + isFontModified);
            Console.WriteLine(&quot;Font Size Modified: &quot; + isFontSizeModified);
            Console.WriteLine(&quot;Font Color Modified: &quot; + isFontColorModified);
            Console.WriteLine(&quot;Horizontal Alignment Modified: &quot; + isHorizontalAlignmentModified);

            // Save the workbook
            workbook.Save(&quot;StyleModifyFlagExample.xlsx&quot;);
        }
```

### See Also

* enum [StyleModifyFlag](../../stylemodifyflag/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


