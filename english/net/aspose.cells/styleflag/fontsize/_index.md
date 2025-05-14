---
title: StyleFlag.FontSize
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Font size setting will be applied
type: docs
url: /net/aspose.cells/styleflag/fontsize/
---
## StyleFlag.FontSize property

Font size setting will be applied.

```csharp
public bool FontSize { get; set; }
```

### Examples

```csharp
// Called: FontSize = true,
public static void StyleFlag_Property_FontSize()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Header 1");
            worksheet.Cells["B1"].PutValue("Header 2");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            // Create a new style object
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
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
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B1");
            range.ApplyStyle(style, styleFlag);

            // Save the workbook
            workbook.Save("StyleFlagExample.xlsx");

            return;
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


