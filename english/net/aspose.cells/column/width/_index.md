---
title: Column.Width
second_title: Aspose.Cells for .NET API Reference
description: Column property. Gets and sets the column width in unit of characters
type: docs
url: /net/aspose.cells/column/width/
---
## Column.Width property

Gets and sets the column width in unit of characters.

```csharp
public double Width { get; set; }
```

### Remarks

For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.

### Examples

```csharp
// Called: worksheet.Cells.Columns[i].Width = 20;
public static void Property_Width()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add new Style to Workbook
            Style style = workbook.CreateStyle();

            // Setting the background color to Blue
            style.ForegroundColor = Color.Blue;

            // Setting Background Pattern
            style.Pattern = BackgroundType.Solid;

            // New Style Flag
            StyleFlag styleFlag = new StyleFlag();

            // Set All Styles
            styleFlag.All = true;

            // Change the default width of first ten columns
            for (int i = 0; i &lt; 10; i++)
            {
                worksheet.Cells.Columns[i].Width = 20;
            }

            // Get the Column with non-default formatting
            ColumnCollection columns = worksheet.Cells.Columns;

            foreach (Column column in columns)
            {
                // Apply Style to first ten Columns
                column.ApplyStyle(style, styleFlag);
            }

            // Saving the Excel file
            workbook.Save(&quot;ColumnCollectionExample.xlsx&quot;);
            workbook.Save(&quot;ColumnCollectionExample.pdf&quot;);
        }
```

### See Also

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


