---
title: ListObject.DisplayName
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets the display name of the table
type: docs
url: /net/aspose.cells.tables/listobject/displayname/
---
## ListObject.DisplayName property

Gets and sets the display name of the table.

```csharp
public string DisplayName { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyDisplayNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);

            // Create a list object
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Set display name and demonstrate its usage
            listObject.DisplayName = "ProductTable";
            Console.WriteLine("List Object Display Name: " + listObject.DisplayName);

            // Save the workbook
            workbook.Save("ListObjectDisplayNameDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


