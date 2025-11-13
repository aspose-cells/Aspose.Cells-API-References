---
title: ListObject.ShowTableStyleFirstColumn
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Indicates whether the first column in the table is the style applied to
type: docs
url: /net/aspose.cells.tables/listobject/showtablestylefirstcolumn/
---
## ListObject.ShowTableStyleFirstColumn property

Indicates whether the first column in the table is the style applied to.

```csharp
public bool ShowTableStyleFirstColumn { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleFirstColumnDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["B4"].PutValue(3.2);

            // Create a list object
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];
            
            // Apply first column style
            listObject.ShowTableStyleFirstColumn = true;
            
            // Save the workbook
            workbook.Save("ListObjectShowFirstColumnStyle.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("File saved with first column style applied to the table.");
        }
    }
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


