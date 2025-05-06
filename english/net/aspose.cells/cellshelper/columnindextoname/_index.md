---
title: CellsHelper.ColumnIndexToName
second_title: Aspose.Cells for .NET API Reference
description: CellsHelper method. Gets column name according to column index
type: docs
url: /net/aspose.cells/cellshelper/columnindextoname/
---
## CellsHelper.ColumnIndexToName method

Gets column name according to column index.

```csharp
public static string ColumnIndexToName(int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |

### Return Value

Name of column.

### Examples

```csharp
// Called: cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
public static void Method_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Populate the worksheet with some data
            for (int i = 0; i &lt; 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row &lt; 10; row++)
            {
                for (int column = 0; column &lt; 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Add a ListObject (table) to the worksheet
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Access the ListColumnCollection of the ListObject
            ListColumnCollection listColumns = table.ListColumns;

            // Demonstrate accessing properties of ListColumnCollection
            Console.WriteLine(&quot;Number of columns in the table: &quot; + listColumns.Count);

            // Access individual ListColumn by index
            ListColumn firstColumn = listColumns[0];
            Console.WriteLine(&quot;First column name: &quot; + firstColumn.Name);

            // Modify the capacity of the ListColumnCollection
            listColumns.Capacity = 10;
            Console.WriteLine(&quot;New capacity of the ListColumnCollection: &quot; + listColumns.Capacity);

            // Save the workbook
            workbook.Save(&quot;ListColumnCollectionExample.xlsx&quot;);
        }
```

### See Also

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


