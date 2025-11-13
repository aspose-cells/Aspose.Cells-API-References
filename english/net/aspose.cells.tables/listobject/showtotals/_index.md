---
title: ListObject.ShowTotals
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets whether this TAble shows total row
type: docs
url: /net/aspose.cells.tables/listobject/showtotals/
---
## ListObject.ShowTotals property

Gets and sets whether this TAble shows total row.

```csharp
public bool ShowTotals { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTotalsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to create a table
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(8);

            // Create a list object/table
            int index = worksheet.ListObjects.Add("A1", "B4", true);
            ListObject table = worksheet.ListObjects[index];

            // Enable totals row and set a calculation
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Save the workbook
            workbook.Save("ListObjectShowTotalsDemo.xlsx");
        }
    }
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


