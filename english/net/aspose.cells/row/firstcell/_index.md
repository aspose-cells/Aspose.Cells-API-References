---
title: Row.FirstCell
second_title: Aspose.Cells for .NET API Reference
description: Row property. Gets the first cell object in the row
type: docs
url: /net/aspose.cells/row/firstcell/
---
## Row.FirstCell property

Gets the first cell object in the row.

```csharp
public Cell FirstCell { get; }
```

### Examples

```csharp
// Called: Cell firstCell = row.FirstCell;
public static void Row_Property_FirstCell()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();

            // Obtaining the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a style object
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

            // Get first row
            Row row = worksheet.Cells.Rows[0];

            // Apply Style to first row
            row.ApplyStyle(style, styleFlag);

            // Setting row properties
            row.Height = 20.0;
            row.IsHidden = false;
            row.IsCollapsed = false;
            row.GroupLevel = 1;
            row.IsHeightMatched = true;

            // Accessing cells in the row
            Cell firstCell = row.FirstCell;
            Cell firstDataCell = row.FirstDataCell;
            Cell lastCell = row.LastCell;
            Cell lastDataCell = row.LastDataCell;

            // Checking if the row is blank
            bool isBlank = row.IsBlank;

            // Checking if the row has custom style
            bool hasCustomStyle = row.HasCustomStyle;

            // Getting the index of the row
            int rowIndex = row.Index;

            // Getting a cell by index
            Cell cellByIndex = row.GetCellByIndex(0);

            // Getting the style of the row
            Style rowStyle = row.GetStyle();

            // Setting the style of the row
            row.SetStyle(rowStyle);

            // Copying settings from another row
            Row sourceRow = worksheet.Cells.Rows[1];
            row.CopySettings(sourceRow, true);

            // Enumerating through cells in the row
            IEnumerator cellEnumerator = row.GetEnumerator();
            while (cellEnumerator.MoveNext())
            {
                Cell cell = (Cell)cellEnumerator.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }

            // Saving the Excel file
            workbook.Save("RowExample.xlsx");
        }
```

### See Also

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


