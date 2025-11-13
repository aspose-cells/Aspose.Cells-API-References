---
title: ListObject.ShowTableStyleLastColumn
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Indicates whether the last column in the table is the style applied to
type: docs
url: /net/aspose.cells.tables/listobject/showtablestylelastcolumn/
---
## ListObject.ShowTableStyleLastColumn property

Indicates whether the last column in the table is the style applied to.

```csharp
public bool ShowTableStyleLastColumn { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleLastColumnDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1.2);

            // Create a list object
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];

            // Set ShowTableStyleLastColumn property
            listObject.ShowTableStyleLastColumn = true;

            // Save the workbook
            workbook.Save("ListObjectShowLastColumnStyle.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("File saved with ShowTableStyleLastColumn enabled.");
        }
    }
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


