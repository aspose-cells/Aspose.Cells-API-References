---
title: Column.IsCollapsed
second_title: Aspose.Cells for .NET API Reference
description: Column property. whether the column is collapsed
type: docs
url: /net/aspose.cells/column/iscollapsed/
---
## Column.IsCollapsed property

whether the column is collapsed

```csharp
public bool IsCollapsed { get; set; }
```

### Examples

```csharp
// Called: column.IsCollapsed = false; // Setting the column collapsed state
public static void Property_IsCollapsed()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add new Style to Workbook
            Style style = workbook.CreateStyle();

            // Setting the background color to Blue
            style.BackgroundColor = Color.Blue;

            // Setting the foreground color to Red
            style.ForegroundColor = Color.Red;

            // Setting Background Pattern
            style.Pattern = BackgroundType.DiagonalStripe;

            // New Style Flag
            StyleFlag styleFlag = new StyleFlag();

            // Set All Styles
            styleFlag.All = true;

            // Get first Column
            Column column = worksheet.Cells.Columns[0];

            // Apply Style to first Column
            column.ApplyStyle(style, styleFlag);

            // Setting additional properties
            column.Width = 20.0; // Setting the column width
            column.IsHidden = false; // Setting the column visibility
            column.IsCollapsed = false; // Setting the column collapsed state

            // Saving the Excel file
            workbook.Save("ColumnExample.xlsx");
            workbook.Save("ColumnExample.pdf");
        }
```

### See Also

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


