---
title: TableToRangeOptions.LastRow
second_title: Aspose.Cells for .NET API Reference
description: TableToRangeOptions property. Gets and sets the last row index of the table
type: docs
url: /net/aspose.cells.tables/tabletorangeoptions/lastrow/
---
## TableToRangeOptions.LastRow property

Gets and sets the last row index of the table.

```csharp
public int LastRow { get; set; }
```

### Examples

```csharp
// Called: LastRow = 9 // Set the last row index of the table
public static void TableToRangeOptions_Property_LastRow()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Populate the worksheet with some data
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Add a ListObject (table) to the worksheet
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Set some properties of the table
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;

            // Create an instance of TableToRangeOptions
            TableToRangeOptions options = new TableToRangeOptions
            {
                LastRow = 9 // Set the last row index of the table
            };

            // Convert the table to a range using the options
            table.ConvertToRange(options);

            // Save the workbook
            workbook.Save("TableToRangeOptionsExample.xlsx");
        }
```

### See Also

* class [TableToRangeOptions](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


