---
title: ListObject.ListColumns
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets the ListColumn list of this table
type: docs
url: /net/aspose.cells.tables/listobject/listcolumns/
---
## ListObject.ListColumns property

Gets the [`ListColumn`](../../listcolumn/) list of this table.

```csharp
public ListColumnCollection ListColumns { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyListColumnsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // Create a list object
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add(0, 0, 9, 4, true);
            ListObject listObject = listObjects[index];
            
            // Enable totals and set calculation for the 5th column
            listObject.ShowTotals = true;
            listObject.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
            
            // Apply table style
            listObject.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleLight4;

            // Save the workbook
            workbook.Save("ListColumnsDemo_out.xlsx");
        }
    }
}
```

### See Also

* class [ListColumnCollection](../../listcolumncollection/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


