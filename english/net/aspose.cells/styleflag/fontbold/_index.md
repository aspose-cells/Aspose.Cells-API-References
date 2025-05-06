---
title: StyleFlag.FontBold
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Font bold setting will be applied
type: docs
url: /net/aspose.cells/styleflag/fontbold/
---
## StyleFlag.FontBold property

Font bold setting will be applied.

```csharp
public bool FontBold { get; set; }
```

### Examples

```csharp
// Called: FontBold = true,
public static void Property_FontBold()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Header 1&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Header 2&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(10);
            worksheet.Cells[&quot;B2&quot;].PutValue(20);
            worksheet.Cells[&quot;A3&quot;].PutValue(30);
            worksheet.Cells[&quot;B3&quot;].PutValue(40);

            // Create a new style object
            Style style = workbook.CreateStyle();
            style.Font.Name = &quot;Arial&quot;;
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Create a new StyleFlag object
            StyleFlag styleFlag = new StyleFlag
            {
                All = true,
                Font = true,
                FontSize = true,
                FontBold = true,
                CellShading = true
            };

            // Apply the style to a range of cells
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(&quot;A1:B1&quot;);
            range.ApplyStyle(style, styleFlag);

            // Save the workbook
            workbook.Save(&quot;StyleFlagExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


