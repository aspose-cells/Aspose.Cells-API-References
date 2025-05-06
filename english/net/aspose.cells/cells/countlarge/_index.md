---
title: Cells.CountLarge
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the total count of instantiated Cell objects
type: docs
url: /net/aspose.cells/cells/countlarge/
---
## Cells.CountLarge property

Gets the total count of instantiated Cell objects.

```csharp
public long CountLarge { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Total Cells Count (Large): &amp;quot; + cells.CountLarge);
public static void Property_CountLarge()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Set default row height
            cells.StandardHeight = 20;
            // Set row height
            cells.SetRowHeight(2, 20.5);

            // Set default column width
            cells.StandardWidth = 15;
            // Set column width
            cells.SetColumnWidth(3, 12.57);

            // Merge cells
            cells.Merge(5, 4, 2, 2);

            // Put values to cells
            cells[0, 0].PutValue(true);
            cells[0, 1].PutValue(1);
            cells[0, 2].PutValue(&quot;abc&quot;);

            // Export data
            object[,] arr = cells.ExportArray(0, 0, 10, 10);

            // Demonstrate some properties
            Console.WriteLine(&quot;Total Cells Count: &quot; + cells.Count);
            Console.WriteLine(&quot;Total Cells Count (Large): &quot; + cells.CountLarge);
            Console.WriteLine(&quot;Min Row with Data: &quot; + cells.MinDataRow);
            Console.WriteLine(&quot;Max Row with Data: &quot; + cells.MaxDataRow);
            Console.WriteLine(&quot;Min Column with Data: &quot; + cells.MinDataColumn);
            Console.WriteLine(&quot;Max Column with Data: &quot; + cells.MaxDataColumn);

            // Iterate through cells
            IEnumerator enumerator = cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine(cell.Name + &quot;: &quot; + cell.Value);
            }

            // Save the workbook
            workbook.Save(&quot;CellsExample.xlsx&quot;);
            workbook.Save(&quot;CellsExample.pdf&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


