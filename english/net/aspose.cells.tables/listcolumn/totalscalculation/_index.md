---
title: ListColumn.TotalsCalculation
second_title: Aspose.Cells for .NET API Reference
description: ListColumn property. Gets and sets the type of calculation in the Totals row of the list column
type: docs
url: /net/aspose.cells.tables/listcolumn/totalscalculation/
---
## ListColumn.TotalsCalculation property

Gets and sets the type of calculation in the Totals row of the list column.

```csharp
public TotalsCalculation TotalsCalculation { get; set; }
```

### Examples

```csharp
// Called: listColumn.TotalsCalculation = TotalsCalculation.Sum;
public static void Property_TotalsCalculation()
        {
            // Create a new workbook and access the first worksheet
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
                for (int column = 0; column &lt; 4; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Add a ListObject (table) to the worksheet
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];
            table.ShowTotals = true;

            // Access the ListColumn and set its properties
            ListColumn listColumn = table.ListColumns[4];
            listColumn.TotalsCalculation = TotalsCalculation.Sum;
            listColumn.Formula = &quot;=[A]&quot;;
            listColumn.Name = &quot;CustomColumn&quot;;
            listColumn.TotalsRowLabel = &quot;Total&quot;;

            // Save the workbook
            workbook.Save(&quot;ListColumnExample.xlsx&quot;);
        }
```

### See Also

* enum [TotalsCalculation](../../totalscalculation/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


