---
title: ListObject.Comment
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets the comment of the table
type: docs
url: /net/aspose.cells.tables/listobject/comment/
---
## ListObject.Comment property

Gets and sets the comment of the table.

```csharp
public string Comment { get; set; }
```

### Examples

```csharp
// Called: table.Comment = &amp;quot;This is a sample table.&amp;quot;;
public static void Property_Comment()
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

            // Set some properties of the ListObject
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;
            table.DisplayName = &quot;SampleTable&quot;;
            table.Comment = &quot;This is a sample table.&quot;;
            table.ShowTableStyleFirstColumn = true;
            table.ShowTableStyleLastColumn = true;
            table.ShowTableStyleRowStripes = true;
            table.ShowTableStyleColumnStripes = true;
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Save the workbook
            workbook.Save(&quot;ListObjectExample.xlsx&quot;);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


